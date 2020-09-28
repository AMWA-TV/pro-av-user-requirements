# Pro AV User Requirements
## Introduction
The following is a list of ProAV user requirements maintained by the Advanced Media Workflow Association (AMWA) on behalf of the Joint Taskforce for Networked Media (JT-NM).
The purpose of this list is to provide a common set of user requirements that may help guide and coordinate the activities of participating JT-NM organizations as they seek to develop standards and specifications to serve the ProAV marketplace.

If you wish to submit a user requirement please ideally submit a Pull Request.  An alternative way to do this is to raise an Issue in this repository.  Your submission will be reviewed by the JT-NM.

## Requirements from the ProAV community
**As a desktop computer user,** I need to be able to see the screen of
my computer clearly. I am often looking at spreadsheets and documents
with thin lines and small text of varying color. I need to be able to do
normal computer things with my mouse, including selecting corners of
windows or double-clicking icons, which often requires me to make
precise movements.

**As an IT Director installing thin clients,** I have a budget to
install thin clients in my call center, which means monitors with
keyboards and mice connected to a virtualized desktop computer that I
control in a server closet. Since 4K monitors are cheap and screen real
estate is appreciated by our staff, I'd like to give everyone 4K
monitors. However, I can't support 10G networks as they are far too
expensive when you add up the costs. Since our staff uses desktop
applications all day long, the quality of the content has to look
pretty much perfect.

* **Requirement:** Must support 8-Bit 4K60 (UHD) video with in 4:4:4 color
sampling at 800Mb/s or less with quality that is excellent (very close
to perfect) with normal desktop content.

***

**As an Esports Gamer,** latency is everything to me. I need my video
displayed on my monitor very quickly. In fact, I pay extra for equipment
that reduces mouse and keyboard latency, and even more for anything that
reduces video latency. I also favor framerate over resolution, because I
crave that feeling of being directly connected to my character which allows
me to achieve better scores.

May need a more ProvAV requirement.

* **Requirement:** Sub-frame latency must be achievable between source and
sync.

***

**As a casual user**, I want to plug my cable into a source and into a
monitor and experience video and audio, as I would if I had used an HDMI
or DisplayPort cable.

* **Requirement:** The solution must support one TX connected directly to
a RX without the need for a network switch or any kind of complex
configuration.

***

**As the owner of a Bar,** I need to show the same television channels
on multiple monitors. Most of the time, this content is HDCP protected
from my cable provider's set top box.

* **Requirement:** Support Multicast display

* **Requirement:** Support Multicast display with HDCP content.

***

**As a User directing live event production including from remote
studio,** I want to make a professional looking video production using
the wide-array of software-based production tools. Because I'm
interacting with people over the internet, I need my latency to be as
low as possible. Because I'm recording the output, I'd like my quality
to be as high as possible. Because my budget is "whatever I can expense
without raising suspicion", my costs need to be very low.

* **Requirement:** Must support working with software-based video
production tools on modern computer hardware.

***

**As an IT Professional,** I expect to be able to purchase networking
equipment from my favorite manufacturer, or vendor. I do not want to
have to buy specialty switches in order to host video on my network.

* **Requirement:** The solution must support using off the shelf network
switches (COTS) that are widely available and not overly expensive.

***

**As a user deploying a handful of devices,** I expect the solution to
be simple to deploy and only require a small inexpensive network,
without the need for dedicated servers or specialty hardware.

* **Requirement:** For small deployments, ad hoc discovery and
synchronization should be achievable. There should not be a need for
dedicated "IPMX servers", a dedicated PTP grandmaster or PTP Aware
Network Switch. An IT expert should not be required to perform the
installation and configuration of IPMX devices, or the network. However,
configuration of IGMP, DHCP and other widely understood protocols is
acceptable

***

**As a user**, I expect to be able to configure a few devices in a
static topology and expect this setup to persist even when devices are
restarted/rebooted.

**As a user** **deploying a large amount of devices**, I accept that I
may require the IT department to be involve to properly configure some
of my network resources. I expect this not to require IPMX technology
specific knowledge and only involve common IT network configuration
knowledge.

**As an IT Professional supporting high-end** **professional or**
**broadcast video productions,** I understand that at times, I need to
buy networking equipment that has unique capabilities, in order to
support extremely high-end video productions with tight requirements for
low-jitter and consistently high bandwidth. Still, I need to be able to
easily move video and control traffic between these networks and the
rest of my network, which also supports video, but not with these
requirements.

* **Requirement:** Customers use video for many purposes and budgets range
from very small to very large, often within the same organization. The
solution must be able to support the full range IT configurations and
capabilities, while providing methods for clean and simple
interoperability.

***

**As a user** **of a purpose built** **or large** **video system**, I
accept that I may benefit from dedicated servers and equipment for my
video system, especially when deploying a large number of devices on my
network, so that my system remains responsive and resilient.

**As a corporate IT professional,** I need to encrypt all video content
on my network, in order to comply with our data security policies. This
includes video content, as well as control traffic.

* **Requirement:** The solution must support carrying encrypted content.

* **Requirement:** The solution must support control traffic encryption.
(this is control not media might be out of scope of this VSF group)

***

**As a digital signage integrator,** I need to create a video wall,
where content is presented synchronously across a matrix of displays.

* **Requirement:** The solution must be able to send a signal to several
receivers to be displayed synchronously. The expectation is for all
displays to show the exact same frame at the same time for all content.

* **Requirement:** The solution must be able to send multiple signals to
one device for aggregation. That device must be able to lineup all the
signals and display them without obvious tearing issues or apparent
de-synchronization.

***

**As an AV Director** **producing** **a live event**, I'm controlling a
production that involves multiple cameras capturing a presenter on the
stage, while I project their magnified image from multiple projectors on
a very large screen that is behind them (IMAG). If the latency is too
high (40-50ms), the viewers in the audience become distracted by poor
lip-sync. Graphics content from laptops and computers are also mixed in,
but synchronization and latency for these sources is less important.

* **Requirement:** Support mixing of synchronous and asynchronous sources.

***

###  Requirements we think are outside the scope of the IMPX VSF activity but which may be within the scope of AMWA or SMPTE activities
(Note: comment reflects that the initial requirments came from the VSF group which was anticipating requirements that may be met by work going on in other industry groups.)

**As** **a User,** I need access to computers, both virtualized and
physical, that are spread throughout my campus. I must be able to switch
between them and control them via mouse and keyboard, braille, or other
HID device.

* **Requirement:** Provide mechanism to virtualize HID devices.

* **Requirement:** Support virtualized, software-only sources.

***

**As a** **Pro AV Integrator**, I need to control and support RS232
devices, which are still popular in the field. With AV over IP, I need
to be able to control them over a network, and often use them in conjunction
with source and display devices.

**As*  a Pro AV Manufacturer,** I have a serial port protocol that I
provide to my users as a method to control/read my device\'s settings.
Because the devices on either end have a serial port, I need to support
this method of communication, even though there is an IP-based network in between.
I need to be able to represent the RS232/422 interfaces on my devices so
that my users can connect devices together that must communicate
serially.

**AS a Pro AV Installer**, I am retrofitting my customer\'s AV system
for IP. We\'re using their existing cameras, which use the ubiquitous
PELCO-D Protocol over a serial port connection. Along with video, I need
to be able to connect this serial port to the receiver, so that my
appliation is able to pan, tilt, and zoom (PTZ) the camera, as required
by the user.

**Requirement:** Provide mechanism to virtualize R232/422 ports, so that
display and source devices that need controlled have an interoperable
way to transfer their control protocols over a network.

***

## From a Broadcaster's point of view
### The following requirements are from Broadcasters who may be looking to use ProAV equipment as part of their professional video workflows

* The solution must operate on a network infrastructure that is
affordable, and that can be designed and configured by the same IT
department that maintains our corporate networking infrastructure.  (No
\$10k network switches, and I don't have a dedicated video IT team -- I
am supported by Corporate IT.)

    (A significant portion of the typical user base for ProAV also
wants this)

* The solution must enable fully software-based solutions.  (My Capital
Equipment budget has been reduced to near zero, but I can expense
software.  Business/financial people now run my business and are in
charge of my department.  Purchasing specialized video hardware is a
strategic investment which our financial people just don't understand or
approve anymore.  But boy are they spending money on software.)

    (Certain users in ProAV also want this but not as prominent as
stated above)

* Compression is a must.  I don't have the spare budget to pay for the
quality of uncompressed, and I can't justify it anyway.

    (In ProAV compression is a must because they want to be able to use
1G/2.5G networks CATx cables etc...Quality is important but the quality
metrics might be different)

* I need better timing than I get with popular proprietary low end
video solutions to enable things such as picture-in-picture and other
production effects, but I simply cannot pay for the "gold-plated SMPTE ST
2110 solution"".  Also, speaking quite frankly, my production team and my
viewers can't tell and don't care if I have some delay or some minor
issues caused by less stringent timing than the gold-plated solution.

    (In ProAV there are several workflows that also need very good
synchronization. A video wall for example, requires each monitor to
display one portion of the same video stream. All monitors must be
synchronized to display the same frame otherwise, there will be obvious
tearing)
