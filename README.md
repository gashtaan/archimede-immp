# Archimede IMMP
I bought the Archimede IMMP 1.1W inverter in the year 2016 and as these devices are quite well designed, soon I became a fan of it. Although, in my experience, they are quite unreliable in sensing the minimum flow. For example, it often runs the pump for tens of minutes when the pipes are completely closed until it realizes that the minimum flow condition already happens. So I've installed a water flow sensor and a power consumption sensor into the system. Then I built a gadget to monitor these parameters to notify when the pump runs when it should not, or stops when it should deliver the water. But that's all I could do with it without modifying the device. As I already have a water flow sensor in the system, my idea is to improve the inverter firmware and hardware to stop the pump right at the moment when the flow actually stops... and this repository is dedicated to this idea.

I have become a collector of these devices. I reverse-engineered both the hardware and the firmware of multiple Archimede IMMP 1.1W devices to find out how they work. Although they're all sold as the same inverter (EF0840), over time, there were significant changes in the hardware. At first, they were based on Freescale MC9S08AW16 MCUs (AW revisions), but later Electroil added optional BlueConnect support and began to sense more runtime parameters, they had to upgrade the MCU to MC9S08GB60A (BC revisions).

So far, I've got my hands on these revisions (according to the labels on PCBs):
* IMMP1.5W-AW-03
* IMMP2.2W-BC-07 (firmware version 4.4)
* IMTP2.2W-BC-10 (firmware version 5.3)
* IMTP2.2W-BC-12 (firmware version 5.4)

I'm still far from the end, so for now, I put here at least the schematics I drew during reverse-engineering the PCBs.
