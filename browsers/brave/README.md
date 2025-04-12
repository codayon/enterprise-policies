# Brave Browser Custom Configuration

This repository provides custom configurations for Brave Browser, applied through two separate files:

1. **GroupPolicy.json** (for Linux systems)
2. **brave.reg** (for Windows systems)

These configurations are designed to enhance privacy, security, and user control by disabling various features and settings in Brave Browser.

## Configuration Overview

- **SyncDisabled**: Disables Brave Sync.
- **BraveAIChatEnabled**: Disables Brave AI Chat functionality.
- **BraveRewardsDisabled**: Disables Brave Rewards (BAT, advertisements).
- **BraveVPNDisabled**: Disables Brave VPN functionality.
- **BraveWalletDisabled**: Disables Brave Wallet.
- **PasswordManagerEnabled**: Disables the built-in password manager.
- **PasswordLeakDetectionEnabled**: Disables password leak detection.
- **PasswordSharingEnabled**: Disables password sharing.
- **PromotionsEnabled**: Disables promotional content or notifications.
- **AutofillAddressEnabled**: Disables address autofill.
- **AutofillCreditCardEnabled**: Disables credit card autofill.
- **MetricsReportingEnabled**: Disables reporting of user metrics.

## Installation

**For Linux Users**:

- Download the GroupPolicy.json file.
- Place the file in the appropriate location on your system:
  - `/etc/brave/policies/managed/` or the equivalent directory for your Brave configuration.
- Check out [brave://policy/](brave://policy/) inside Firefox.

**For Windows Users**:

- Download the brave.reg file.
- Double-click the file to add the settings to your system’s registry.
- Restart Brave Browser for the changes to take effect.

### Reference

- [Group Policy](https://support.brave.com/hc/en-us/articles/360039248271-Group-Policy)
