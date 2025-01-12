contracts-v4

🦑 Smart contracts for Ocean Protocol v4. https://hyperocean.ai Ocean v4 is part of the Ocean Protocol toolset.

This is in beta state and you can expect running into problems. If you run into them, please open up a new issue.

-📚 Installation
-🏄 Quickstart
-Features
-Publisher Flow
-Roles Diagram
-Functions you will need
-Bundle functions
-🦑 Development and testing
-🏛 License

📚 Installation
For quick installation of the contract ABIs:

Javascript/Typescript
npm install @oceanprotocol/contracts
Python
pip3 install ocean-contracts
⚙️ Usage
By default, Python does not support importing json files directly, so it is recommended to use json-sempai package in order to automatically importing ABIs/json artifacts.

pip3 install json-sempai
# install the ocean-contracts package.
from jsonsempai import magic
from artifacts import address
Overview

![oceancontractsa](https://github.com/user-attachments/assets/bb441924-b714-4dd1-8eba-1c30519b6e15)


🏄 Quickstart
Features
Base IP is now represented by an NFT, from which a datapublisher can create multiple ERC20s representing different type of access for the same dataset.

Help Ocean Community Monetize: there's a swap fee for the Ocean Community, if Ocean or allied tokens are the basetoken in a pool, Ocean Community will receive 0.1% swap fee, otherwhise it will be 0.2%.

Flexibility
Based on ERC721 and ERC20 templates to provide different features

Introduce an advanced Fee Structure both for Market and Provider runners.

Roles Administration: there are now multiple roles for a more flexible administation both at NFT and ERC20 levels

Key-value store in the NFT contract : NFT contract can be used to store custom key-value pairs (ERC725Y standard)

Multiple NFT template support: the Factory can deploy different types of NFT templates

Multiple datatoken template support: the Factory can deploy different types of Datatoken templates

Publisher Flow
Interaction flow from DataPublisher point of view.

Go to publisher flow

Roles Diagram
How roles are handled in the v4.

Go to roles diagram

Functions you will need
Selection of most common functions.

Go to functions

Bundle functions
Helper functions which can perform multiple steps in 1 call.

Go to helpers

If you have any difficulties with the quickstarts, or if you have further questions about how to use the contracts please reach out to us on Discord.

If you notice any bugs or issues with this repo please open an issue on github. -->

The ocean.js and ocean.py libraries wrap contracts in JavaScript and Python respectively. They each have quickstart guides.

🦑 Development and Testing
Run hardhat in a new terminal:

export ALCHEMY_URL="https://eth-mainnet.alchemyapi.io/v2/XXXXXXXX"
npm install
npx hardhat node
Open a new terminal to run the tests:

export ALCHEMY_URL="https://eth-mainnet.alchemyapi.io/v2/XXXXXXXX"

npm run test:full
# same thing, but with coverage reporting
npm run test:full:cover
Unit Tests
You can execute just unit tests with:

npm run test:unit
Flow Tests
You can execute just flow tests with:

npm run test:flow
🏛 License
Copyright ((C)) 2023 Ocean Protocol Foundation

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
