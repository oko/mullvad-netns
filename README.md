# `mullvad-netns`

Creates a Linux network namespace that has connectivity to a Mullvad Wireguard VPN endpoint.

## Installation

```
git clone https://github.com/oko/mullvad-netns
cd mullvad-netns
sudo make install
```

## Usage

Create a configuration file:

```
CONFIG_PRIVATE_KEY=$YOUR_WIREGUARD_PUBLIC_KEY
CONFIG_ACCOUNT_ID=$YOUR_MULLVAD_ACCOUNT_ID
```

Then run `mullvad-netns` (via `sudo` as it requires privileges):

```
sudo mullvad-netns $NETNS_NAME $CONFIG_FILE
```
