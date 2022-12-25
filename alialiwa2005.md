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

Initially, I planned to build another project powered by the UK-made Raspberry Pi, but unfortunately I was unable to get my hands on them on time for Winter of Making 2023 due a major shortage of Raspberry Pis at the time of writing... so I had to resort to an alternative SBC. 

The Librecomputer SBC isn't as widely-supportive nor as well-documented as the Raspberry Pi.

However, the Librecomputer should be able to execute basic NAS functions and should be applicable for this build. OpenMediaVault has an officially supported image released by Librecomputer, so that's what we'll use. 

OpenMediaVault is an open-source Linux-based Network Attached Storage operating system, so it's a good choice for our project's software.

## Plan

For this project, you'll need some identical SBCs. You can use Librecomputer's LePotato for a tighter budget, or use Renegade boards for their hardware performance perks. I'll use Librecomputer's Renegade boards. They have a gigabit ethernet port, unlike the other Librecomputer SBCs, which are limited to 100mbit/s via ethernet port. A higher bandwidth capacity is useful for faster serving and uploading of files, especially larger ones, over LAN. What's also interesting is their form-factor, which is identical to that of a Pi 3 Model B... this is true for the LePotato as well.

Aside from these, you also need basic accessories, like power supplies (Minimum 5v 2a via MicroUSB), storage (MicroSD), and ethernet cables.

You'll also need a laptop or PC for imaging the microSD cards for booting OpenMediaVault on the Librecomputer SBCs.

Another optional but recommended item is: A network switch, so that all the boards connect to the ethernet switch, which ultimately uses a single port of your router. You'll need a 5+ port router, including a port for the network switch to be linked to a router.

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
| Ethernet Network Switch                 | https://amzn.to/3hTmGUv               | $19.79  |

| Subtotal, Sales Tax, Shipping           |                                       |         |
| --------------------------------------- | ------------------------------------- | ------- |
| Item Subtotal                           |                                       | $269.77 |
| Item Subtotal + NYC Sales Tax (8.875%)     | ($241.97)(108.875%)                   | $293.72 |
| Renegade SBCs Shipping                  | USPS First Class                      | $5.01   |

| Grand Total |
| ----------- |
| $298.73     |
