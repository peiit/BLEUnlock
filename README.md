# BLEUnlock

BLEUnlock is a small menu bar utility that locks and unlocks your Mac with your iPhone, Apple Watch, or any other Bluetooth Low Energy device.

This document is also available in [Japanese](README.ja.md).

## Features

- No iPhone app is required
- Works with any BLE devices that periodically send signal
- Unlocks your Mac for you when the device is near Mac, no need to enter password again
- Locks your Mac when the device is away from Mac
- Optionally wakes from display sleep state
- Optionally pauses and unpauses iTunes playback when you're away and back
- Password is securely stored in Keychain
- Uses Hardened Runtime and notarized by Apple
![](https://i.imgur.com/i9Rj44q.png)

## Requirements

- Mac with Bluetooth Low Energy support
- macOS 10.13 (High Sierra) or later
- iPhone 5s or later, Apple Watch (all), or other BLE device that transmits
signal periodically

## Installation

Download zip file from [Releases](https://github.com/ts1/BLEUnlock/releases),
unzip and copy to Applications folder.

On the first launch, it asks your login password,
which is required to unlock the lock screen.
It's safe because it's stored in Keychain. 

Then it asks for permission for Accessibility.
In System Preferences, click the lock icon to unlock and turn BLEUnlock on.
This permission is also required to unlock the lock screen.

Finally, from the menu bar icon, select "Device".
It starts scanning nearby BLE devices.
Select your device, and you're done!

## Troubleshooting

If it fails to unlock, check BLEUnlock is turned on in "System Preferences" →
"Security & Privacy" → "Privacy" → "Accessibility".
If it is already on, try turning it off and on again.

If it asks for permission to access its own password, click "Always Allow",
because it is needed while the screen is locked.

If "Signal is lost" occurs frequently, turn Bluetooth of Mac off then on.
Or use a device that sends signal more frequently.

## Acknowledgement

Icon is based on `lock-open.svg` downloaded from materialdesignicons.com,
which is originally designed by Google LLC and licensed under Apache License
version 2.0.

## License

MIT

Copyright © 2019 Takeshi Sone.
