# this is a Remix backup Folder

This is a Remix project folder that contains the default scripts, contracts, and test cases. Additionally, two custom contracts have been added, which have been compiled and deployed.

## Table of Contents

- [Token Contract](https://github.com/ZafeerMahmood/Remix/blob/main/.workspaces/remixDefault_Fyp/contracts/MorarableToken.sol)
- [Trading Contract](https://github.com/ZafeerMahmood/Remix/blob/main/.workspaces/remixDefault_Fyp/contracts/MorarableMarketContract.sol)

# Setup

1. open remix.ethereum.org and in Contracts add your own or copy these

# Usage

1. Open Remix and navigate to the project folder and add your Contracts.
2. Complie with Remix
3. Run and Test with Remix
4. finaly deploy it with an injected metamask account with any test eth eg goerlieth and view it on https://goerli.etherscan.io/


# Example Code :
1. Token Contract.
   ```solidity
   contract <YOUR CONTRACT NAME> is ERC721 {
    using Counters for Counters.Counter;
    Counters.Counter private _tokenIds;

    constructor()ERC721("<YOUR TOKEN NAME>","<YOUR TOKEN SYMBOL"){}

    struct Item{
        uint256 id;
        address creator;
        string uri;
    }
   ```
2. Trading Contract.
   ```solidity
   contract <YOUR CONTRACT NAME> {
    struct AuctionItem {
        uint256 id;
        address tokenAddress;
        uint256 tokenId;
        address payable seller;
        uint256 askingPrice;
        bool  isSold;
    }

   ```


