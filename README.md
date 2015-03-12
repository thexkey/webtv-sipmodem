# WebTV SIP-based Software Modem

This is a software modem written in C that uses a SIP gateway to listen for incoming calls and allows a WebTV to establish a data connection to the Internet. 

I'm using OpenSIPS to parse the SIP protocol, pjmedia to handle most of the audio compression, and SpanDSP to handle some of the early DSP in the dialup handshake.

Depending on the ATA device you use, it may or may not work well. All depends on network latency, jitter and audio quality produced by ATA device.  Dialup protocols weren't designed for VoIP.

This should run on Linux or Solaris as long as you have mgetty and pppd installed.

ATA devices tested:

- MeshPotato Phone 2.0
- Unlocked BasicTalk HT701
- Unlocked Vonage VDV21

UltimateTV boxes can use an ethernet adapter as long as you have the correct ROM image and set the proper bit in the NVRAM. I'll explain when I fix up the code to put on here.

I'll add the code soon, I promise. Nerd approved.
