# Monerujo
Another Android Monero Wallet for Monero
	**(not
    Monero Classic,
    Monero-Classic,
    Monero Zero,
    Monero Original,
    Monero C,
    Monero V)**

### QUICKSTART
- Download the APK for the most current release [here](https://github.com/m2049r/xmrwallet/releases) and install it
- Alternatively add our F-Droid repo https://f-droid.monerujo.io/fdroid/repo with fingerpint ```A8 2C 68 E1 4A F0 AA 6A 2E C2 0E 6B 27 2E FF 25 E5 A0 38 F3 F6 58 84 31 6E 0F 5E 0D 91 E7 B7 13``` to your F-Droid client
- Run the App and select "Generate Wallet" to create a new wallet or recover a wallet
- Advanced users can copy over synced wallet files (all files) onto sdcard in directory Monerujo (created first time App is started)
- See the [FAQ](doc/FAQ.md)

## Translations
Help us translate Monerujo! You can find instructions [On Taiga](https://taiga.getmonero.org/project/erciccione-monero-localization/wiki/monerujo), and if you need help/support, open an issue or contact the Localization Workgroup. You can find us on the freenode channel `#monero-translations`, also relayed on [MatterMost](https://mattermost.getmonero.org/monero/channels/monero-translations), and matrix/riot.

### Disclaimer
You may lose all your Moneroj if you use this App. Be cautious when spending on the mainnet.

### Random Notes
- Based off monero v0.11.1.0
- currently only android32 (runs on 64-bit as well)
- works on the testnet & mainnet
- sync is slow due to 32-bit architecture
- use your own daemon - it's easy
- screen stays on until first sync is complete
- Monerujo means "Monero Wallet" according to https://www.reddit.com/r/Monero/comments/3exy7t/esperanto_corner/

### TODO
- see taiga.getmonero.org & issues on github

### Issues / Pitfalls
- Users of Zenfone MAX & Zenfone 2 Laser (possibly others) **MUST** use the armeabi-v7a APK as the arm64-v8a build uses hardware AES
functionality these models don't have.
- You should backup your wallet files in the "monerujo" folder periodically.
- Also note, that on some devices the backups will only be visible on a PC over USB after a reboot of the device (it's an Android bug/feature)
- Created wallets on a private testnet are unusable because the restore height is set to that
of the "real" testnet.  After creating a new wallet, make a **new** one by recovering from the seed.
The official monero client shows the same behaviour.

### HOW TO BUILD
No need to build. Binaries are included:

- openssl-1.0.2l
- monero-v0.12
- boost_1_58_0

If you want to build them yourself (recommended) check out [the instructions](doc/BUILDING-external-libs.md)

Then, fire up Android Studio and build the APK.

### Donations
- Address: 4AdkPJoxn7JCvAby9szgnt93MSEwdnxdhaASxbTBm6x5dCwmsDep2UYN4FhStDn5i11nsJbpU7oj59ahg8gXb1Mg3viqCuk
- Viewkey: b1aff2a12191723da0afbe75516f94dd8b068215f6e847d8da57aca5f1f98e0c
