# A Novel Approach to 802.11 Probe Request Analysis, Part V
Hello All,  It's been a while since my last post, [A Novel Approach to 802.11 Probe Request Analysis, Part IV](https://medium.com/@underneaththec/a-novel-approach-to-802-11-probe-request-analysis-part-iv-0e8f8aea6343)

Since then, I've standardized on the Raspberry Pi Zero W2 with a USBHat as a platform, Got [Blue2thprinting](https://github.com/darkmentorllc/Blue2thprinting) up and running, switched to mysql instead of sqlite and gave a talk, which can be found [here](https://youtu.be/bhOlNRRP_YA).

Some interesting findings, to avoid more threat actors, I've decided not to enumerate them, publicly at at least, and switched focus to the PII and PII fragments which could be used for seeds for OSINT pivots.  Also, by examining sequence numbers I've found, SSID Bursts, aka probing rounds, hop channels in the middle of a burst.  In order to get a full picture of how probing works, one must monitor all (most) wifi channels.  This means multiple raspberry pi's with usb hat's all talking to a central mysql server.  

I got this up and running but it turns out tshark can hog resources.  I tried a python alternative but found that it maxes out the CPU and cranks the heat up.  Pi Zero's start throttling cpu at 80 degrees C.  I'm also wondering if SDcard write speed is an issue, So I'm in the process of upgrading those.

You can follow allow with the project [here](https://github.com/maxxsyntax/probeprint2).

That's it for now.  I'll provide an update when there's something interesting to share.



