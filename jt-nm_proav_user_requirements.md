# JT-NM Pro AV User Requirements

## Introduction

The following is a list of ProAV user requirements maintained by the Advanced Media Workflow Association (AMWA) on behalf of the Joint Task Force on Networked Media (JT-NM), which owns the list.

The purpose of this list is to provide a common set of user requirements that coordinate the activities of JT-NM member organizations as they develop standards and specifications to serve the ProAV marketplace.

If you wish to submit a user requirement please submit a Pull Request.  An alternative way to do this is to raise an Issue in this repository.  Your submission will be reviewed by the JT-NM.

While it is possible for individuals to submit user stories to this repository, we *strongly* prefer that you work through the appropriate committee of a JT-NM organization, such as the Audio Engineering Society (AES), the Advanced Media Workflow Association (AMWA), the European Broadcasting Union (EBU), the Society of Motion Picture and Television Engineers (SMPTE) or the Video Services Forum (VSF), to have your requirements vetted by one of these organizations.

## Requirements from the ProAV community

**As a desktop computer user,** I need to be able to see the screen of my computer clearly. I am often looking at spreadsheets and documents with thin lines and small text of varying color. I need to be able to do normal computer things with my mouse, including selecting corners of windows or double-clicking icons, which often requires me to make precise movements.

**As an IT Director installing thin clients,** I have a budget to install thin clients in my call center, which means monitors with keyboards and mice connected to a virtualized desktop computer that I control in a server closet. Since 4K monitors are cheap and screen real estate is appreciated by our staff, I'd like to give everyone 4K monitors. However, I can't support 10G networks as they are far too expensive when you add up the costs. Since our staff uses desktop applications all day long, the quality of the content has to look pretty much perfect.

* **Requirement:** Must support 8-Bit 4K60 (UHD) video with in 4:4:4 color sampling at 800Mb/s or less with quality that is excellent (very close to perfect) with normal desktop content.

***

**As an Esports Gamer,** latency is everything to me. I need my video displayed on my monitor very quickly. In fact, I pay extra for equipment that reduces mouse and keyboard latency, and even more for anything that reduces video latency. I also favor framerate over resolution, because I crave that feeling of being directly connected to my character which allows me to achieve better scores.

May need a more ProAV requirement.

* **Requirement:** Sub-frame latency must be achievable between source and sync.

***

**As a casual user**, I want to plug my cable into a source and into a monitor and experience video and audio, as I would if I had used an HDMI or DisplayPort cable.

* **Requirement:** The solution must support one TX connected directly to a RX without the need for a network switch or any kind of complex configuration.

***

**As the owner of a Bar,** I need to show the same television channels on multiple monitors. Most of the time, this content is HDCP protected from my cable provider's set top box.

* **Requirement:** Support Multicast display

* **Requirement:** Support Multicast display with HDCP content.

***

**As a User directing live event production including from remote studio,** I want to make a professional looking video production using a wide-array of software-based production tools. Because I'm interacting with people over the internet, I need my latency to be as low as possible so that the latency I experience in the rest of the system doesn't overwhelm the production. Because I'm recording the output, I'd like my quality to be as high as possible. Because my budget is "whatever I can expense without raising suspicion", my costs need to be very low.

* **Requirement:** Must support working with software-based video production tools on modern computer hardware.

***

**As an IT Professional,** I expect to be able to purchase networking equipment from my favorite manufacturer, or vendor. I do not want to have to buy specialty switches in order to host video on my network.

* **Requirement:** The solution must support using off the shelf network switches (COTS) that are widely available and not overly expensive.

***

**As a user deploying a handful of devices,** I expect the solution to be simple to deploy and only require a small inexpensive network, without the need for dedicated servers or specialty hardware.

* **Requirement:** For small deployments, ad hoc discovery and synchronization should be achievable. There should not be a need for dedicated "IPMX servers", a dedicated PTP grandmaster or PTP Aware Network Switch. An IT expert should not be required to perform the installation and configuration of IPMX devices, or the network. However, configuration of IGMP, DHCP and other widely understood protocols is acceptable

***

**As a user**, I expect to be able to configure a few devices in a static topology and expect this setup to persist even when devices are restarted/rebooted.

**As a user deploying a large amount of devices**, I accept that I may require the IT department to be involve to properly configure some of my network resources. I expect this not to require IPMX technology specific knowledge and only involve common IT network configuration knowledge.

**As an IT Professional supporting high-end professional or broadcast video productions,** I understand that at times, I need to buy networking equipment that has unique capabilities, in order to support extremely high-end video productions with tight requirements for low-jitter and consistently high bandwidth. Still, I need to be able to easily move video and control traffic between these networks and the rest of my network, which also supports video, but not with these requirements.

* **Requirement:** Customers use video for many purposes and budgets range from very small to very large, often within the same organization. The solution must be able to support the full range IT configurations and capabilities, while providing methods for clean and simple interoperability.

***

**As a user of a purpose built or large video system**, I accept that I may benefit from dedicated servers and equipment for my video system, especially when deploying a large number of devices on my network, so that my system remains responsive and resilient.

**As a corporate IT professional,** I need to encrypt all video content on my network, in order to comply with our data security policies. This includes video content, as well as control traffic.

* **Requirement:** The solution must support carrying encrypted content.

* **Requirement:** The solution must support control traffic encryption. (this is control not media might be out of scope of this VSF group)

***

**As a digital signage integrator,** I need to create a video wall, where content is presented synchronously across a matrix of displays.

* **Requirement:** The solution must be able to send a signal to several receivers to be displayed synchronously. The expectation is for all displays to show the exact same frame at the same time for all content.

* **Requirement:** The solution must be able to send multiple signals to one device for aggregation. That device must be able to lineup all the signals and display them without obvious tearing issues or apparent de-synchronization.

***

**As an AV Director producing a live event**, I'm controlling a production that involves multiple cameras capturing a presenter on the stage, while I project their magnified image from multiple projectors on a very large screen that is behind them (IMAG). If the latency is too high (40-50ms), the viewers in the audience become distracted by poor lip-sync. Graphics content from laptops and computers are also mixed in, but synchronization and latency for these sources is less important.

* **Requirement:** Support mixing of synchronous and asynchronous sources.

### Unreliable, Shared, WAN, or WiFi networks and alignment

**As a user visiting a huddle room with my laptop**, I'd like to share my screen with the room's monitor and AV system. I have a normal laptop, which may lack an ethernet port. I expect to be able to discover the AV system from WiFi in this room from my laptop and share my display. I don't expect the experience to rival the direct connection I get with a cable, but I'd like it to be close and to not be distractingly bad.

**As a visitor in a huddle room with a smartphone**, I'd like to share my screen with the room's monitor and AV system. My phone is connected to WiFi and I would expect to see a simple and easy way to connect and view it on the display with reasonable latency and decent quality.

> **Note:** For the above two use cases: *Reasonable latency* means that it's not impossible to carry on a two-way conversation with someone who is using the same or similar technology as me on the other end. *Decent quality* needs to be defined.

**As an IT manager**, I have many users that bring their own devices including laptops, tablets and phones. My user's expectations are that they can connect wirelessly. The trouble is, there are many different ways to do that in the consumer world, but in the Pro AV world, we need to manage account and device access. Our televisions are not signed into someone's Apple or Google account. We need a common, vendor and platform independent standard for streaming content from devices over wireless networks.

At the same time, we do not want this technology to be completely separated from the transport we do over wired networks. We still need wired networks because there are many time where we need lower latency or we need to have mezzanine or even raw quality. We do not want to have totally separated control planes or timing mechanism, even though we understand that streams are not always compatible across profiles.

I need video and audio to be aligned when they come from the same source. For me, I do not expect to be able to synchronize video or audio from multiple sources over WiFi networks or with my wired network.

**As a computer user**, I don't want my network to stop working when someone starts streaming video over WiFi. I also don't want to make the video or audio stutter while I'm using WiFi. I'd like latency to be as low as possible, so that I can use wireless networks in more applications where I would otherwise use wired network technology.

**As an AV system designer or consultant or purchasing agent**, I'm very interested in open standards whenever I can choose them. However, I also need to save money and solve real problems. It would be great if an open standard for AV over IP could be supported by existing cameras and other gear that I own, especially cameras and gateways that already support h264. Ideally, it would be possible to support IPMX through a firmware update.

**As a digital signage system designer for a large transportation project,** I am looking for flexibility. For example, sometimes I care about latency because the signage is triggered by transportation events and having some assurances about when signs must change in response to those events is important. Other times, latency or even reliability does not matter as much as overcoming cabling, environmental, or other infrastructure concerns. In those scenarios, a wireless connection is much better. In all cases, I'd like to use the same control plane API, and for the system to understand which devices can connect to each other.

**I'm an in-store brand manager for a fast food chain,** and I need to support drive through displays. Very often, running a network cable out to these displays is difficult. It would be simplest if we could connect to our outside displays wirelessly, so that we don't have to deal with installing a new network cable to the display. Also, we need relatively low latency, so there is not too much added delay between when the order taker updates the order and when the customer sees it.

**As a video technician recording high school sports,** I follow our teams to away games, including soccer, basketball and football. In these facilities, I do not have access to their network or any cabling infrastructure. Running my own cables is a pain and often I'm very limited as to where I can run them. Ideally, I could arrive on location with a small fly pack that included 3-4 WiFi cameras, which I could use to shoot the game, controlling them with pan-tilt-zoom (PTZ) controls on a panel. Because I'm shooting sports, latency in the transport can be very annoying because the delay makes it difficult to precisely control the camera as the action moves around.

Also, I need the cameras to be somewhat in sync, as I will be switching between two cameras that are recording the same action from different perspectives. Finally, I also have a wired camera that I use, which sits right next to me, along with a couple of microphones that are wired. I need to be able to keep everything in sync with the WiFi cameras, even though this camera typically has much lower latency than my WiFi cameras.

**As a KVM computer user with a 1GbE connection to a switch from my target computer,** I have multiple desktop images and file traffic that shares the connection. I want to stream both desktops over my AV over IP network, but I want to minimize the bandwidth used for transmission so that I can have more room for file and web traffic.

**As a digital signage installer,** I need to stream four 4K feeds over a single 1GbE for an 8K video wall supported by four 4K receivers. Latency is not a concern, if it is less than a few seconds. The quality needs to be very good, but most viewers will be standing a few feet away, so visually perfect video is not a requirement.

**As a manufacturer with existing h264 cameras and gateway devices,** I would like to participate in IPMX. If I could retrofit my devices to be IPMX compliant, then my users could benefit from standards based interoperability much more quickly.

* **Requirement:** There is a profile that works over unstable or other less-than ideal physical transport, including some set of WiFi, 5G, satellite, or other public/shared pipe networks.
* **Requirement:** There is a profile that works over wireless and nicely interoperates with the rest of the (wired/low-latency) system. Systems can reason about latency for stream re-alignment.
* **Requirement:** There is a codec that can compress the content as much as is required for the bandwidth constrained network with measurable latency.
* **Requirement:** There is a codec that can compress the content as much as is required for the bandwidth constrained network, while still retaining reasonable quality and adds no more than X seconds of latency. Reasonable latency means latency low enough that a typical camera operator can operate a PTZ camera during a basketball game.
* **Requirement:** There is equipment that people can buy or already have that is or can be made compatible with the open standard.
* **Requirement:** Latency over WiFi can be measured, so that realignment with the rest of the system can be achieved.

### Control

**As a system engineer for a multi-campus organizations** and I am tasked with deploying, configuring and maintaining the equipment in my AV system. I have thousands of pieces of gear from countless manufacturers. I have hundreds of little semi-autonomous systems that use the same network. Some of this equipment uses different transport standards (IPMX, ST 2110, AES67, AVB, some legacy proprietary protocols).

I need to be able to automate/script the deployment of this equipment without having to accommodate every manufacturer's special method for changing settings over a network. A similar need exists for monitoring and logging this equipment. I need to know what equipment I have, the state of that equipment, and a way common to understand what it does and to manipulate it over the network using scripts, control systems and other mechanisms for control.

Finally, if something should go wrong or a device enters into a state that I need to track (a device stops recording, an RX device is no longer receiving video or is dropping packets, device is too hot...) I need to be notified.

* **Requirement** There is a consistent API (same API for every compliant device) for identifying AV equipment on a network. User can discover the manufacturer, serial number, model number, firmware revision and any other identifying information related to the equipment.

* **Requirement** There is a consistent API for configuring devices over a network. The user can understand what the settings are for the device. The meaning of each setting is understandable within the API itself. Settings may be read only or settable by an authorized client.
* **Requirement** There is a consistent and IT-friendly / familiar method for monitoring the state of compliant AV devices. There should be a method for subscribing (or some similar method) to state changes and alarms.
* **Requirement** There is a consistent way to control the device, generally. The user can manipulate the state of the device, limited by permissions and device capability, through a consistent network API.

### Out-of-box experience and accessibility

**As a curious professional or amateur or pro-sumer**, I am excited about building media systems with open standards IP. Currently, I use proprietary solutions that are free to download, but that system has limitations and it isn't a true open standard. I'm open to trying something that is an open standard and might have some features that the current options lack. What's the fastest way that I can try out IPMX? Where's the free/open source package that lets me play with it?

I don't expect to do everything for free, but I expect to be able to do some things right away and for free, especially since proprietary options let me do that.

**As a person hosting an event that wants to share content with guests** I need a barrier-free way for my guests to receive my content, without having to pay any kind of licensing fee. My expectation is that while producing great looking content with low-latency should probably cost at least some money, everyone should be able to view the content without paying anything.

* **Requirement:** There is or at least can be (with volunteer help) a baseline, freely available IPMX repo for people to play with and experiment with IPMX, without paying anyone money. It may be limited to some defined profile limit. Example: 4:2:2 HD 8-BIT video.

* **Requirement:** Anyone can watch any produced content without paying a royalty for anything associated with the transport.

### Resolution Scaling

**As a director or network operations center employee,** I use multi-viewers to monitor many inputs at once on a single large display. I don't typically see any one input full screen. I typically need to see 6-12 inputs at the same time, but it might be more. With so many inputs, network bandwidth becomes a concern. Also, when viewing my multi-viewer feeds, the timing is important. If the preview windows are delayed from the real content, it makes it impossible make decisions based on what I can see in the window.

**As a sports venue AV system designer,** I have feeds that originate as 4K flows for my production system, but I also need them to stream to 1080p displays, such as our digital signage system. I would rather not duplicate these flows only to support 1080p.

* **Requirement:** A method for providing multiple resolutions of a single flow, without consuming significantly more bandwidth on the network than the highest resolution flow would have been, by itself.
* **Requirement:** Each version of the flow is in sync with every other version.
* **Requirement:** Receiving a lower resolution flow consumes much less bandwidth than receiving the full flow.
* **Requirement:** A typical use case would be: 4k, 1080p and qHD (1/4 1080p) available on the network.

### High Bit Depth for Direct View LED Video Walls

**As an AV Integrator specializing in high-value retail, transportation, and simulation experiences,** I am tasked with deploying visually compelling LED video walls. These walls are composed of multiple LED cabinets (ranging from 10-20 units) that require precise and high-quality video signal distribution.

Key Requirements

* **High Bit Depth:** The system must support very high bit depths, potentially up to 16-20 bits per pixel, to drive the LED tiles effectively. This ensures rich color depth and nuanced visual detail, crucial for high-end applications that employ high-dynamic range LED technology.
* **Efficient Data Transmission:** Each LED cabinet's video data should be transmitted as a separate video stream.

> **Note:** This approach aligns with the established 4x FHD stream use cases but extends it further in terms of coding efficiency.

* **Network Compatibility:** The solution must utilize existing standard Ethernet network infrastructure, operating within the bandwidth constraints of 1-10G. This compatibility ensures ease of integration into current systems without the need for extensive network upgrades.
* **Priority on Bandwidth and Cost:** In this scenario, achieving low bandwidth utilization and cost-effectiveness is paramount. These factors take precedence over low latency and visually lossless compression.
* **Software-Friendly Deployment:** For ease of deployment and maintenance, the solution must be amenable to software-based implementations. This requirement is key for ensuring that the system is flexible, upgradable, and easy to manage.

#### Implications

This use case represents an advanced application of IPMX, targeting scenarios where exceptional, very high-dynamic range visual quality is required, along with efficient use of network resources. It reflects the growing demand for high-fidelity, networked AV solutions in settings where the visual experience is a critical aspect of the overall value proposition.

## Requirements we think are outside the scope of the IPMX VSF activity but which may be within the scope of AMWA or SMPTE activities

> **Note:** comment reflects that the initial requirements came from the VSF group which was anticipating requirements that may be met by work going on in other industry groups.

**As a User,** I need access to computers, both virtualized and physical, that are spread throughout my campus. I must be able to switch between them and control them via mouse and keyboard, braille, or other HID device.

* **Requirement:** Provide mechanism to virtualize HID devices.

* **Requirement:** Support virtualized, software-only sources.

***

**As a Pro AV Integrator**, I need to control and support RS232 devices, which are still popular in the field. With AV over IP, I need to be able to control them over a network, and often use them in conjunction with source and display devices.

**As a Pro AV Manufacturer,** I have a serial port protocol that I provide to my users as a method to control/read my device's settings. Because the devices on either end have a serial port, I need to support this method of communication, even though there is an IP-based network in between. I need to be able to represent the RS232/422 interfaces on my devices so that my users can connect devices together that must communicate serially.

**As a Pro AV Installer**, I am retrofitting my customer's AV system for IP. We're using their existing cameras, which use the ubiquitous PELCO-D Protocol over a serial port connection. Along with video, I need to be able to connect this serial port to the receiver, so that my application is able to pan, tilt, and zoom (PTZ) the camera, as required by the user.

**Requirement:** Provide mechanism to virtualize R232/422 ports, so that display and source devices that need controlled have an interoperable way to transfer their control protocols over a network.

***

## From a Broadcaster's point of view

### The following requirements are from Broadcasters who may be looking to use ProAV equipment as part of their professional video workflows

* The solution must operate on a network infrastructure that is affordable, and that can be designed and configured by the same IT
department that maintains our corporate networking infrastructure.  (No \$10k network switches, and I don't have a dedicated video IT team -- I am supported by Corporate IT.)

> **Note:** A significant portion of the typical user base for ProAV also wants this.

* The solution must enable fully software-based solutions.  (My Capital Equipment budget has been reduced to near zero, but I can expense software.  Business/financial people now run my business and are in charge of my department.  Purchasing specialized video hardware is a strategic investment which our financial people just don't understand or approve anymore.  But boy are they spending money on software.)

> **Note:** Certain users in ProAV also want this but not as prominent as stated above.

* Compression is a must.  I don't have the spare budget to pay for the quality of uncompressed, and I can't justify it anyway.

> **Note:** In ProAV compression is a must because they want to be able to use 1G/2.5G networks CATx cables etc...Quality is important but the quality metrics might be different.

* I need better timing than I get with popular proprietary low end video solutions to enable things such as picture-in-picture and other production effects, but I simply cannot pay for the "gold-plated SMPTE ST 2110 solution"".  Also, speaking quite frankly, my production team and my viewers can't tell and don't care if I have some delay or some minor issues caused by less stringent timing than the gold-plated solution.

> **Note:** In ProAV there are several workflows that also need very good synchronization. A video wall for example, requires each monitor to display one portion of the same video stream. All monitors must be synchronized to display the same frame otherwise, there will be obvious tearing.