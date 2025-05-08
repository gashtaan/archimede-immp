# Archimede IMMP
This project is related to the Archimede IMMP series pump inverters made by Electroil.

In my experience, these inverters are quite unreliable in sensing the minimum flow. The inverter itself is bad at sensing it - for example, it often runs the pump for tens of minutes when the pipes are completely closed until it realizes the minimum flow condition already happens. I had to build another gadget to monitor the inverter to notify me when the pump runs when it should not or stops when it should deliver the water. As I already have a water flow sensor in the system to monitor it, my idea was to improve the inverter to stop the pump right at the moment when the flow actually stops.

For now, I've reverse engineered the hardware only, so I put at least schematics here.
