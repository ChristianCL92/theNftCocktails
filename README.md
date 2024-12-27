# NFT Cocktails Metadata

This repository contains the metadata and images for the UniqueCocktailNfts NFT collection deployed on the Ethereum Sepolia testnet.

## Repository Structure

```
theNftCocktails/
├── metadata/
│   ├── Cocktails/          # JSON metadata files for each NFT
│   │   ├── WHITERUSSIAN.json
│   │   ├── AMARETTOSOUR.json
│   │   └── ...
│   └── images/             # Image files for each cocktail NFT
│       ├── white-russian.webp
│       ├── amaretto-sour.webp
│       └── ...
```

## Metadata Format

Each cocktail NFT's metadata follows the OpenSea metadata standard and includes:

- name: The cocktail's display name
- description: Detailed description of the cocktail
- image: Direct link to the cocktail's image
- attributes: Array of traits including:
  - Category
  - Base Spirit
  - Glass Type
  - Difficulty
  - IBA Official status
  - Year Created
  - Ingredients
  - Instructions
  - Garnish
  - Serving Style
  - Alcohol Content

Example metadata structure:
```json
{
  "name": "Amaretto Sour",
  "description": "A sweet and sour cocktail...",
  "image": "https://raw.githubusercontent.com/ChristianCL92/theNftCocktails/main/metadata/images/amaretto-sour.webp",
  "attributes": [
    {
      "trait_type": "Category",
      "value": "Sour"
    },
    ...
  ]
}
```

## Usage

This repository serves as the metadata storage for the UniqueCocktailNfts smart contract deployed at: `0xBAFfEbe1652c2164F3a2Aaaa3dc3DF0974b848b7`

The metadata is accessed through the baseURI in smart contract:
```
https://raw.githubusercontent.com/ChristianCL92/theNftCocktails/main/metadata/Cocktails/
```

## Related Repositories

- Frontend Application: https://github.com/ChristianCL92/nft-cocktails-frontend 
- Smart Contract: https://github.com/ChristianCL92/nft-cocktails-contract

## Note

This repository is part of an educational project focused on blockchain technology and NFTs. The content is for demonstration purposes only.
