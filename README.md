# Archimede IMMP
This project is related to the Archimede IMMP series pump inverters made by Electroil.

In my experience, these inverters are quite unreliable in sensing the minimum flow. The inverter itself is bad at sensing it - for example, it often runs the pump for tens of minutes when the pipes are completely closed until it realizes the minimum flow condition already happens. I had to build another gadget to monitor the inverter to notify me when the pump runs when it should not or stops when it should deliver the water. As I already have a water flow sensor in the system to monitor it, my idea was to improve the inverter to stop the pump right at the moment when the flow actually stops.

Unfortunately, the MCU (MC9S08AW60 or MC9S08GB60A) flash is protected, so far I'm not able to dump out of it. It's a shame, it would be the best option to just reverse engineer the existing firmware and rewrite it to satisfy my needs. This way, I have to start from the scratch... begin with a proper testing environment.

For now, I've reverse engineered the hardware only, so I put at least schematics here.
