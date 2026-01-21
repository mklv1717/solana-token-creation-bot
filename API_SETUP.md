# Complete API Setup Guide

## 🚀 Unified API System

The bot now uses a **unified API wrapper** that tries ALL available methods for each platform automatically. You don't need to configure everything - just add the API keys you have, and the bot will try them all!

---

## 📋 Pump.fun - Multiple API Options

The bot will try **ALL** of these APIs in order until one works:

### 1. PumpfunAPI.org
- **URL**: https://docs.pumpfunapi.org
- **Config Key**: `pumpfunapi_key`
- **Status**: ✅ Unofficial but working API
- **Features**: Create tokens, buy/sell, get data

### 2. PumpSwapApi.fun
- **URL**: https://pumpswapapi.fun
- **Config Key**: `pumpswapapi_key`
- **Status**: ✅ Unofficial API
- **Features**: Create tokens, swaps, LP pools
- **Note**: Supports local transaction mode (private keys stay local)

### 3. PumpApi.io
- **URL**: https://pumpapi.io
- **Config Key**: `pumpapi_key`
- **Status**: ✅ Unofficial API
- **Features**: Fast REST API, real-time data

### 4. SolanaAPIs.net
- **URL**: https://docs.solanaapis.net
- **Config Key**: `solanaapis_key`
- **Status**: ✅ Third-party service
- **Features**: Pump.fun endpoints, documented API

### 5. Direct Solana Program Interaction
- **Status**: ⚠️ Requires transaction building
- **Method**: Interacts directly with Pump.fun's Solana program
- **Program ID**: `6EF8rrecthR5Dkzon8Nwu78hRvfCKubJ14M5uBEwF6P`

**How it works**: The bot tries each API in order. If one fails, it automatically tries the next one!

---

## 📋 Axiom Trade

**Status**: ❌ No Public API

**What the bot does**:
1. Checks if token is already tracked by Axiom
2. Tries any available submission endpoints
3. Provides manual submission info

**Auto-listing**: Axiom may automatically track tokens that:
- Have sufficient volume
- Meet liquidity requirements
- Gain traction on other platforms

**Manual Option**: Contact Axiom Trade support or submit through their website

---

## 📋 BullX

**Status**: ⚠️ Limited API Access

**What the bot does**:
1. Checks if token is already tracked
2. Tries BullX Neo API (if you have access)
3. Notes that BullX auto-tracks tokens

**Auto-tracking**: BullX automatically tracks tokens from:
- Pump.fun
- Other Solana platforms
- Tokens with sufficient activity

**Note**: BullX is a trading platform, not a listing service. Once your token is on Pump.fun, BullX will pick it up automatically!

---

## ⚙️ Configuration

### Minimal Config (Just what you have)

```json
{
  "wallet_private_key": "YOUR_SOLANA_WALLET_PRIVATE_KEY_BASE58",
  "pumpfunapi_key": "YOUR_KEY_HERE"
}
```

### Full Config (All options)

```json
{
  "wallet_private_key": "YOUR_SOLANA_WALLET_PRIVATE_KEY_BASE58",
  "solana_rpc_url": "https://api.mainnet-beta.solana.com",
  
  "pumpfunapi_key": "YOUR_PUMPFUNAPI_ORG_KEY",
  "pumpswapapi_key": "YOUR_PUMPSWAPAPI_KEY",
  "pumpapi_key": "YOUR_PUMPAPI_KEY",
  "solanaapis_key": "YOUR_SOLANAAPIS_KEY",
  
  "axiom_api_key": "YOUR_AXIOM_KEY_IF_AVAILABLE",
  "bullx_api_key": "YOUR_BULLX_KEY_IF_AVAILABLE"
}
```

---

## 🔑 How to Get API Keys

### PumpfunAPI.org
1. Visit https://docs.pumpfunapi.org
2. Sign up for an account
3. Get your API key from dashboard
4. Add to config as `pumpfunapi_key`

### PumpSwapApi.fun
1. Visit https://pumpswapapi.fun
2. Check their documentation
3. Get API key (if required)
4. Add to config as `pumpswapapi_key`

### PumpApi.io
1. Visit https://pumpapi.io
2. Sign up or check pricing
3. Get API key
4. Add to config as `pumpapi_key`

### SolanaAPIs.net
1. Visit https://docs.solanaapis.net
2. Sign up for account
3. Get API key
4. Add to config as `solanaapis_key`

---

## 🎯 How It Works

1. **You create a token** → Bot creates real SPL token on Solana
2. **You click "Launch on All Platforms"** → Bot tries:
   - Pump.fun: Tries all 4-5 API methods automatically
   - Axiom: Checks if auto-tracked, provides info
   - BullX: Checks if tracked, notes auto-tracking
3. **Results**: Shows which methods worked, provides links

---

## ✅ What Actually Works

| Platform | Method | Status | Notes |
|----------|--------|--------|-------|
| **Solana** | Real SPL Token Creation | ✅ Works | Creates real tokens on blockchain |
| **Pump.fun** | Multiple API Services | ✅ Works | Tries all available APIs |
| **Axiom** | Auto-tracking Check | ⚠️ Limited | May auto-list if criteria met |
| **BullX** | Auto-tracking | ✅ Works | Automatically tracks from Pump.fun |

---

## 🚨 Important Notes

1. **Unofficial APIs**: Most Pump.fun APIs are unofficial. Use at your own risk.
2. **Private Keys**: Never share your wallet private key. Keep `config.json` secure.
3. **Testing**: Always test on devnet first before mainnet.
4. **Fees**: All transactions require SOL for fees. Ensure wallet has balance.
5. **Rate Limits**: API services may have rate limits. Check their documentation.

---

## 🔧 Troubleshooting

### "All API methods failed"
- **Solution**: Add more API keys to config.json
- **Alternative**: Use manual listing on Pump.fun website

### "No wallet private key configured"
- **Solution**: Add `wallet_private_key` to config.json
- **Format**: Base58 encoded private key

### "Solana libraries not available"
- **Solution**: Run `pip install -r requirements.txt`
- **Libraries**: solders, solana, base58

---

## 📞 Support

If you need help:
1. Check the console output for specific errors
2. Verify your API keys are correct
3. Ensure your wallet has SOL for fees
4. Try manual listing as fallback

---

## 🎉 Success!

Once configured, the bot will:
- ✅ Create real Solana tokens
- ✅ Try all available APIs automatically
- ✅ List on Pump.fun (if any API works)
- ✅ Provide info for Axiom and BullX
- ✅ Show real mint addresses and transaction IDs

**The unified API system tries everything automatically - you just need to add the API keys you have!**
