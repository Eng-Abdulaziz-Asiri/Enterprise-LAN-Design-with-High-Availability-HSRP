# Enterprise LAN with HSRP

A practical Cisco Packet Tracer project demonstrating High Availability in a local network.

## 🛠️ Technologies Used
- **HSRP:** For router redundancy (Active/Standby).
- **VLANs (10 & 20):** For network segmentation.
- **Static Routing:** To connect to an external ISP.

## 🚀 How to Test it Yourself
1. Open the `.pkt` file in Cisco Packet Tracer.
2. Open the Command Prompt on any PC and ping the ISP: `ping 10.0.0.2`
3. **The Failover Test:** While the ping is running, turn off the main router (`R1-Active`) or delete its cable.
4. Click the **Fast Forward Time (>>)** button at the bottom of the screen.
5. The ping will resume automatically, proving that the standby router took over successfully!

## 🔍 Quick Verification Command
Run this command on the routers to see the HSRP state:
`show standby brief`
