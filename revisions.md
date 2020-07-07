---
title: "HW Revision and Variations"
permalink: /ap2_revisions/
layout: page
nav_order: 1
---
# C15 vs C18 Hardware Revision

## What's different
The key differences are the microcontrolleres used. In the `C15` revision,
two HT32F52342, LQFP48 are used for the matrix and led controllers; however,
in the `C18` revision they used two HT32F52352, LQFP64. These two are very close
in software perspective, but the pin mapping is slightly different. For details
of the micro controller themselves, please refer to Holtek's documentation. But
in summary, the HT32F52352 comes with 128K flash and 16K ram, where the
HT32F52342 comes with only 64K flash and 8K ram.

## How do I tell?
There are various indicators as of which revision is which.

### Case
Flipping you keyboard over, C15 version seems to have "obinslab" engraved in the
circle where as C18 has "Anne Pro".

### USB ID
If you happen to have an Linux / macOS, you can identify this easily by using lsusb
or system info. When the keyboard is in IAP mode, C15 revision will show up as having
`04d9:8008` as its USB VendorID and ProductID pair. Where as the C18 revision has
`04d9:8009`.