# PennyFi powered by Aragon OSx <a href="https://aragon.org/"><img align="right" src=".github/assets/aragon.svg" height="80px" /></a>




## Quick start

Install with `yarn` and launch the app with `yarn start`. By default, the app is configured to connect to the Ethereum Goerli testnet.

For connecting to other chains / deployments, a few useful npm scripts are provided:

- Ethereum Mainnet: `yarn start:mainnet` will launch the app, configured to connect to the Ethereum mainnet
- Local development: `yarn start:local` will launch the app, configured to connect to our [aragen](https://github.com/aragon/aragen) local development environment. It will also use the local IPFS daemon, if it detects one exists. If you're using the [aragonCLI](http://github.com/aragon/aragon-cli), you'll want to run this to connect to its local chain.

**Note**: Windows users may need to install the [windows-build-tools](https://www.npmjs.com/package/windows-build-tools) before installing this project's dependencies.

More [configuration options](docs/CONFIGURATION.md) are available, and depending on your needs, you may find the [frontend development setup guide](docs/FRONTEND_SETUP.md) helpful.

## Releases

The Aragon client is automatically deployed to IPFS with each new commit to `master`, via [Fleek](https://fleek.co/). The latest builds are available at [`client.aragon.org`](https://client.aragon.org/) or through an IPFS gateway, like [`ipfs.io/ipns/client.aragon.org`](https://ipfs.io/ipns/client.aragon.org/).

### aragonPM

"Checkpointed" releases, tagged in our [releases page](https://github.com/aragon/aragon/releases), are published on-chain onto the `aragon.aragonpm.eth` aragonPM repository for all supported Ethereum environments (mainnet and Goerli testnet).

For a long time (2018-2020), these releases were our primary "official" builds. With [Fleek](https://fleek.co/), however, we now relegate these on-chain deployments as historical backups in case a user wants to use an older version.

#### Secrets

A number of environment secrets are required during publishing and these are sometimes different per network.

You may either specify these secrets as environment variables or use a `.env`.


#### Contributors

Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):


## Re-usable foundations

Amongst other dependencies, the Aragon client is built upon these packages that you may also find useful for your projects:

- [aragonUI](https://github.com/aragon/aragon-ui): React component library used to build user interfaces within the [Aragon design system](https://blog.aragon.org/introducing-aragonds-the-new-aragon-design-system/)
- [token-amount](http://github.com/aragon/token-amount): utility class for encapsulating and formatting a token amount
- [use-inside](https://github.com/aragon/use-inside): React utility that allows a component to be aware of being "inside" the subtree of another component
- [use-token](https://github.com/aragon/use-token): React utility for fetching information related to tokens on Ethereum
- [use-viewport](https://github.com/aragon/use-viewport): React utility providing the current window size and convenient functions for responsive apps
- [use-wallet](https://github.com/aragon/use-wallet): React utility aiming to make the integration between your dapp and your users' web3 wallets as straightforward as possible
- [web3-react](https://github.com/NoahZinsmeister/web3-react): a simple, maximally extensible React framework for supporting arbitrary web3 wallets
