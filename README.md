Titanic's End - Ice, Lights, and Music
=================

Project Repository for Titanic's End Electronics

- [Facebook Group](https://www.facebook.com/groups/1434882210102871/)
- [Crowdtilt](https://www.crowdtilt.com/campaigns/titanics-end)
- [Issues](https://github.com/nottombrown/IceLightsAndMusic/issues) (get involved!)

![Sweet Rendering](https://cloud.githubusercontent.com/assets/306655/3239022/981f72f2-f102-11e3-9e56-e604742f7924.jpg)

# MVP

Burning man starts on **Aug 24th**. When we arrive, we must have the following:

- [ ] LEDs along the exterior of the frame
- [ ] LEDs throughout the interior
- [ ] A sound system (with small speakers in the interior)
- [ ] A generator that provides reliable power

We'd like to keep the entire electronics budget below $5k

# Roadmap

https://www.google.com/calendar/embed?src=q6iqtt235h5isporsgrl2aepcs%40group.calendar.google.com&ctz=America/Los_Angeles

# Wiring

![titanics_end_diagram](https://cloud.githubusercontent.com/assets/306655/3335592/cf1e1274-f817-11e3-9934-029488f935b8.png)

If you want to contribute, feel free to edit the [omnigraffle file](https://www.dropbox.com/s/9u4l34wucbv1rlj/titanics_end_diagram.graffle)

# LEDs

Quick math for the size of the car

- Height ~3.5m
- Length ~ 6m
- Width ~ 2.5m

This gives us a total perimiter of 17m and a total area of 59.5m^2

## LED strips
I've had several recommendation for [waterproof WS2812B strips](http://www.aliexpress.com/item/BLACK-PCB-5m-DC5V-WS2812B-led-pixel-srip-IP68-30pcs-WS2812B-M-with-30pixels-reverse-protection/926778326.html)

Each strip has the following specs:

- $30.00 per strip (plus shipping)
- 150 LEDs per strip
- 5m per strip
- 120 degree emitting angle
- 36 watts per strip
- 2550 lumens (17 lumens/LED)

If we get 70 of them and cut them into 50 LED segments, some napkin math would give us:

- 210 strip segments (each 166 cm long and drawing 12 watts)
- 350 total meters of strips
- 2520 watts
- 10,500 total LEDs
- 178,500 lumens (As bright as about 300 x 60W halogen bulbs)
- ~$2.5k

## LED Controllers

Fadecandy: https://github.com/scanlime/fadecandy

Purchasable on [Adafruit](http://www.adafruit.com/products/1689). Each one has the following specs:

- Can control up to 8 strip segments (each up to 64 pixels long, ours are 50)
- $25 (plus shipping)

If we get 26 of them it means:

- We can control 208 segments
- We have to solder 208 segments
- It will cost $720

# Nodes

Seems like there are four main LED sections that need power and control

- Left side
- Right side
- Front & Interior
- Back & DJ booth

In each of those sections, we should have a *node*. The node will contain a power supply and a USB hub, and should be protected so that it does not get damaged.

## USB hubs

We want a powered hub with at least 8 USB ports.

## Power Supplies

We need a power supply that provides the following

- 12V
- 768 watts (A side node has 64 segments, each drawing 12 watts)

The best one I've found is this [Rosewill 1000W](http://www.amazon.com/Rosewill-RBR1000-M-1000-Watt-Certified-compatible/dp/B003J89V0A/ref=sr_1_8?s=pc&ie=UTF8&qid=1403177907&sr=1-8&keywords=power+supply) which looks great but is a bit pricey. I'd be up for other suggestions.

# Brain

We should bring an old macbook, which will let us debug things on the fly. If it breaks, it will be replaceable by other macbooks. Uses 85 watts

# Sound System

Kan Bros have a large speaker system, I'd estimate it at 2000W

# Generator

I'd like to use inverter generators because they're quiet and efficient. We already have one [3100W Champion](http://www.amazon.com/gp/product/B00BBDCE1S/ref=oh_details_o06_s00_i00?ie=UTF8&psc=1), I think we should get a second. One will be dedicated lights, and the other dedicated audio.
