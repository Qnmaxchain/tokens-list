# Contributing to QNMAX Token List

Thank you for your interest in adding your token to the official QNMAX token list! This guide will walk you through the process.

## How to Add Your Token

### Step 1: Fork the Repository

1. Go to [https://github.com/qnmaxchain/tokens-list](https://github.com/qnmaxchain/tokens-list)
2. Click the "Fork" button in the top right corner
3. This creates a copy of the repository in your GitHub account

### Step 2: Clone Your Fork

```bash
git clone https://github.com/qnmaxchain/tokens-list.git
cd tokens-list
```

### Step 3: Add Your Token

Edit the `tokens-info.json` file and add your token information:

```json
{
  "name": "QNMAX Token List",
  "version": {
    "major": 1,
    "minor": 0,
    "patch": 0
  },
  "tokens": [
    // ... existing tokens ...
    {
      "address": "0xYourTokenContractAddress",
      "symbol": "YOUR",
      "name": "Your Token Name",
      "decimals": 18,
      "chainId": 265,
      "logoURI": "https://your-domain.com/logo.png"
    }
  ]
}
```

### Step 4: Token Requirements

Your token must meet these requirements:

#### Technical Requirements
- ✅ **Valid Contract**: Deployed on QNMAX Mainnet (Chain ID: 265)
- ✅ **ERC-20 Standard**: Implements standard ERC-20 functions
- ✅ **Verified Contract**: Source code verified on QNMAX Explorer
- ✅ **No Proxy Contracts**: Direct implementation preferred
- ✅ **Sufficient Liquidity**: At least $1,000 in liquidity

#### Information Requirements
- ✅ **Accurate Details**: Symbol, name, and decimals must match contract
- ✅ **Logo Image**: High-quality PNG/SVG, 200x200px minimum
- ✅ **HTTPS Logo URL**: Logo must be hosted on HTTPS
- ✅ **Unique Symbol**: No conflicts with existing tokens

#### Community Requirements
- ✅ **Active Project**: Regular development activity
- ✅ **Community Presence**: Active social media or community
- ✅ **Documentation**: Clear project documentation
- ✅ **No Scam/Rug**: Legitimate project with real utility

### Step 5: Logo Guidelines

Your token logo should:
- Be a PNG or SVG file
- Have a transparent background
- Be at least 200x200 pixels
- Be under 100KB in file size
- Be hosted on a reliable HTTPS URL
- Represent your project professionally

### Step 6: Submit Your Pull Request

1. **Commit your changes**
   ```bash
   git add tokens-info.json
   git commit -m "Add [TOKEN_SYMBOL] token"
   git push origin main
   ```

2. **Create Pull Request**
   - Go to your forked repository on GitHub
   - Click "New Pull Request"
   - Fill out the PR template with required information

3. **PR Template**
   ```markdown
   ## Token Addition Request
   
   **Token Information:**
   - Name: Your Token Name
   - Symbol: YOUR
   - Contract Address: 0x...
   - Decimals: 18
   - Chain ID: 265
   
   **Verification:**
   - [ ] Contract is verified on QNMAX Explorer
   - [ ] Token has sufficient liquidity (>$1,000)
   - [ ] Logo meets requirements
   - [ ] All information is accurate
   
   **Links:**
   - Website: https://yourproject.com
   - Explorer: https://explorer.qnmax.com/address/0x...
   - Logo URL: https://yourproject.com/logo.png
   
   **Additional Information:**
   Brief description of your project and token utility.
   ```

### Step 7: Review Process

1. **Automated Checks**: Our bot will verify basic requirements
2. **Community Review**: 48-hour community review period
3. **Team Review**: QNMAX team final approval
4. **Merge**: Token added to official list

## Review Criteria

### ✅ Approved Tokens
- Legitimate DeFi projects
- Gaming and NFT tokens
- Utility tokens with real use cases
- Established projects with community

### ❌ Rejected Tokens
- Meme coins without utility
- Suspected scam projects
- Tokens with malicious code
- Duplicate or copycat projects
- Tokens with locked/paused functions

## After Approval

Once your token is approved:
- It will appear in the QNMAX DEX token selector
- Users can easily find and trade your token
- Your token gains visibility in the QNMAX ecosystem

## Token Updates

To update your token information:
1. Fork the repository again
2. Make your changes
3. Submit a new pull request
4. Reference the original PR in your description

## Common Issues

### Contract Not Found
- Ensure your contract is deployed on QNMAX Mainnet (Chain ID: 265)
- Double-check the contract address

### Logo Not Loading
- Verify the logo URL is accessible via HTTPS
- Check that the image meets size requirements
- Ensure the URL doesn't require authentication

### Duplicate Symbol
- Choose a unique symbol not already in use
- Consider adding a suffix if necessary

## Need Help?
- **Telegram**: [t.me/qnmax](https://t.me/qnmaxchain)
- **Email**: tokens@qnmax.com
- **GitHub Issues**: [Create an issue](https://github.com/qnmaxchain/tokens-list/issues)

## Example Token Entry

```json
{
  "address": "0x1234567890123456789012345678901234567890",
  "symbol": "EXAMPLE",
  "name": "Example Token",
  "decimals": 18,
  "chainId": 265,
  "logoURI": "https://example.com/logo.png"
}
```

Thank you for contributing to the QNMAX ecosystem! 🚀
