#NO LONGER USING THIS, I found a betters soloution:

Simply import wallet connect via:
`import WalletConnectProvider from '@walletconnect/web3-provider/dist/umd/index.min.js';`
and to get the types working, make a d.ts file with:
`declare module '@walletconnect/web3-provider/dist/umd/index.min.js' {
  import WalletConnectProvider from '@walletconnect/web3-provider/dist/esm/index';
  export default WalletConnectProvider
}`

# WalletConnect build browsers

As WalletConnect 1.6.5 does not build with rollup, this a a webpack browser pre-built which can be used in rollup.

This Exports WalletConnectClient, WalletConnectProvider, and QRCodeModal
