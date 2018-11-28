# Cryptocoin Address Validator

Use this code tell if a given address is valid for a given cryptocoin.

The design goals of this library are:
  * Simplicity
  * Security

This code has no dependencies and defines a single function
`isValidAddress(coin,address)` which returns true or false.

The variables `coin` and `address` are assumed to be potentially-hostile user input. The main purpose of this library is to prevent easily-detectable invalid addresses from ever getting to lower-level libraries or coin daemons (like `bitcoind`).

Use at your own risk! This is currently being developed and not ready
for production use.

# Examples

    isValidAddress("BTC","notvalid") # returns false

# Supported coins

  * BTC
  * LTC
  * KMD (and asset chains)
  * HUSH
  * VRSC
  * ZEC
  * ZCL
  * PIVX
  * ETH
  * ETC
  * DASH
  * GAME
  * EMC2

# License

MIT

