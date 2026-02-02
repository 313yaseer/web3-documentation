# Transaction Failed - Troubleshooting Guide

Common reasons why transactions fail and how to fix them.

## Common Error Messages

### Error: "Insufficient funds for gas"

**Cause**: Not enough ETH to pay gas fee

**Solution:**
1. Check your ETH balance
2. Add more ETH to your wallet
3. Retry transaction

**How much ETH needed:**
- Simple transfer: ~0.002 ETH
- Token swap: ~0.01 ETH
- Complex contract: ~0.02 ETH

---

### Error: "Transaction underpriced"

**Cause**: Gas price too low for current network conditions

**Solution:**
1. Increase gas price in MetaMask
2. Click "Edit" on gas settings
3. Select "Aggressive" or "Market" priority
4. Retry transaction

---

### Error: "Nonce too low"

**Cause**: Transaction nonce conflict (usually from pending transactions)

**Solution:**
1. Open MetaMask
2. Click Settings → Advanced
3. Click "Reset Account"
4. Retry transaction

⚠️ Note: This clears pending transactions but doesn't affect funds

---

### Error: "Execution reverted"

**Cause**: Smart contract rejected the transaction (slippage, permissions, etc.)

**Solution:**
1. For swaps: Increase slippage tolerance (try 1%, 3%, 5%)
2. Check token approval status
3. Verify you have sufficient balance
4. Check contract documentation for specific requirements

---

### Error: "Out of gas"

**Cause**: Gas limit set too low for transaction complexity

**Solution:**
1. Increase gas limit in transaction settings
2. Typical limits:
   - Simple transfer: 21,000
   - Token transfer: 65,000
   - Swap: 150,000-300,000
   - Complex contract: 500,000+
3. Retry transaction

---

## General Troubleshooting Steps

### 1. Check Network Status

Visit:
- Etherscan: https://etherscan.io/
- Ethereum Gas Tracker: https://etherscan.io/gastracker

Look for:
- Current gas prices
- Network congestion
- Recent successful transactions

### 2. Verify Wallet Connection

1. Wallet unlocked? ✅
2. Correct network selected? (Ethereum Mainnet) ✅
3. Website connected? ✅
4. Sufficient ETH for gas? ✅

### 3. Clear Browser Cache

1. Close all tabs
2. Clear browser cache
3. Restart browser
4. Reconnect wallet

### 4. Update MetaMask

1. Check for MetaMask updates
2. Update if available
3. Restart browser

### 5. Try Again Later

If network is congested:
- Wait 1-2 hours
- Try during off-peak hours (weekends, late night UTC)

## Still Not Working?

### Contact Support

Provide these details:
1. **Transaction hash** (if available)
2. **Error message** (exact text or screenshot)
3. **Wallet address**
4. **What you were trying to do**
5. **Browser and MetaMask version**

### Emergency Actions

**If transaction is stuck:**
1. You can "speed up" or "cancel" in MetaMask
2. Click the pending transaction
3. Choose "Speed Up" (higher gas) or "Cancel"

**If funds seem missing:**
1. Don't panic - check block explorer
2. Go to: https://etherscan.io/address/YOUR_ADDRESS
3. Look for your transaction
4. If confirmed, funds are safe (may need to refresh app)

## Prevention Tips

✅ Always test with small amounts first
✅ Keep extra ETH for gas fees
✅ Use current gas price recommendations
✅ Verify contract addresses
✅ Double-check transaction details before confirming
