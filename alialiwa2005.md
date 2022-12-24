---
name: "@alialiwa2005"
project: "NAStack"
---

# Project Name
NAStack
## Summary

I'm going to build a NAS-Stack, I'll call it "NAStack."

NAStack is a DIY network attached storage build, specifically designed for redundant file storage across multiple NAS nodes saving and serving files within a single unified stack.

Through building this project, I hope to learn more about redundancy, specifically disk redundancy through nodes; for serving images, videos, and documents.

I hope to gain experience from this build in order to build a more versatile cluster of Raspberry Pis (which are currently hard to find during a critical shortage at the time of writing) soon.

Initially, I planned to build a full-on DIY AWS with Raspberry Pis, but unfortunately, there is a major shortage of Raspberry Pis, and I was unable to get my hands on them on time for Winter of Making 2023... so I had to resort to an alternative SBC. Unlike the well-documented and widely-supportive Raspberry Pi, which is the "original" and "the gold standard" arm SBC for most home tinkerers, the Librecomputer SBC isn't fully supportive of the software (and some hardware) requirements needed for a DIY AWS project powered by Kubernetes or isn't as well-documented as the Raspberry Pi in that use-case.

However, the Librecomputer should support some basic NAS functions and should be applicable for a backup build in this case. OpenMediaVault has an officially supported image released by Librecomputer, so it should be able to work.


## Plan

For this project, you'll need some identical SBCs. I'll use 4 Librecomputer Renegade Boards. They have a gigabit ethernet port, unlike the other Librecomputer SBCs, which have 100mbit/s ports. This is useful for faster serving and uploading of files, especially larger ones, over LAN.

Aside from these, you also need basic accessories, like power supplies (Minimum 5v 2a via MicroUSB), storage (MicroSD), and ethernet cables.

You'll also need a laptop or PC for imaging the microSD cards for booting OpenMediaVault on the Librecomputer SBCs.

Some other optional but recommended items are:

- A network switch, so that they all connect to the ethernet switch, which ultimately links to your router via a 
single network cable.

---

Step 1: Order materials (full list at the bottom), then await items' arrival.

Step 2: Image OpenMediaVault to SD cards on your laptop/PC.

Step 3a: Customize cluster stand parts (make it look stylish!) 

Step 3b: Mount SBCs to cluster stand platforms.

Step 3c: Stack platforms and attach pillars via screws until they are secure.

Step 4: Insert SD cards into boards, attach Ethernet cables, then power the boards with MicroUSB cables.

Step 5: Experiment & Hack with OpenMediaVault! You can try testing out some plugins. (One way you might link up nodes together is: 3 nodes' network-shared storage mounted to 1 serving node, which will act as the "proxy" or "primary central server.")

## Budget

| Product                                 | Supplier/Link                         | Cost    |
| --------------------------------------- | ------------------------------------- | ------- |
| 4 Libre Computer Renegade SBCs          | https://bit.ly/3VhXMvx                | $200    |
| USB Power Supply                        | https://amzn.to/3PNXNq0               | $29.99  |
| 4 MicroSD Cards                         | (Already Own)                         | $0      |
| Cluster Stand                           | https://amzn.to/3HYMERp               | $19.99  |

| Item Subtotal                           |                                       | $249.98 |
| Item Total + NYC Sales Tax (8.875%)     | ($241.97)(108.875%)                   | $272.17 |

| Renegade SBCs Shipping                  | USPS First Class                      | $5.01   |

| Grand Total                             |                                       | $277.18 |
