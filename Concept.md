# Concept

* Is identical in UI and function on both iOS and Android.
* Supports segwit (both P2SH and bech32) as standard.
 * Legacy addresses supported through manual creation, but considered deprecated.
* Supports Lightning (initially "disabled" or "hidden" but can be enabled by advanced users or in a later update when ready).
 * Lightning support is to be "transparent" to the user.
 * No manual channel management required.
 * Manual channel management supported, but discouraged.
* Supports setting of custom fees in addition to calculated fees (both as sat/byte as well as absolute figures).
* Allows selection of UTXOs for inputs as well as address to be used for change.
* Supports batch payments (multiple output destinations).
* Does not require manually selecting UTXOs or change addresses.
* Supports selection of provider for exchange rate displays.
* Either very cheap or free.
 * No advertising in the UI or other such degradation of user experience.
 * Wallet provided either at low cost on app stores to recoup development effort or completely free.
 * I'd consider (but am far from convinced at this stage) about micropayments on Lightning as a monetisation system along the lines of 1 satoshi per transaction being directed to the developer or similar.
* Can use external centralised services (such as exchange rate providers) but never requires an external centralised service (such as a user database or "key storage" or similar)
 * When an external service such as an exchange rate provider is used, failure to access that provider gracefully degrades the usage (for example, showing a statement that exchange rates can not be found right now) but doesn't prevent usage of core application features.
* Supports a "view only wallet" for both simple addresses and public keys from which multiple addresses are derived.
* Has the ability to import/sweep wallets using all major/common seed word lists, private key QR codes, and so on.
* Is purely a BTC wallet and doesn't provide options for dealing with other cryptocurrencies (forks of the project could be made for other cryptos; but the main project should not support anything other than BTC)

Overall, I want something ultimately simple to use for the typical user, where the only obvious UI elements are "My balance", "send BTC", and "Receive BTC"; but through advanced optional features hidden away behind UI elements an advanced user can adjust almost everything they could possibly want to. No decisions are made unilaterally by the application or connected systems without the ability for the user to change them manually should they so choose.
