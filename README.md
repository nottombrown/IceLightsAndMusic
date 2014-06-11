Titanic's End - Ice, Lights, and Music
=================

Project Repository for Titanic's End Electronics

- [Facebook Group](https://www.facebook.com/groups/1434882210102871/)
- [Crowdtilt](https://www.crowdtilt.com/campaigns/titanics-end)
- [Issues](https://github.com/nottombrown/IceLightsAndMusic/issues) (get involved!)

# MVP

Burning man starts on **Aug 24th**. When we arrive, we must have the following:

- [ ] LEDs along the exterior of the frame
- [ ] LEDs throughout the interior
- [ ] A sound system (with small speakers in the interior)
- [ ] A generator that provides reliable power

We'd like to keep the entire electronics budget below $5k

# Roadmap

https://www.google.com/calendar/embed?src=q6iqtt235h5isporsgrl2aepcs%40group.calendar.google.com&ctz=America/Los_Angeles

# Exterior LEDs

The current plan would have the following specs

- ~175,000 lumens
- ~2600 watts
- ~$3k

## LED strips
I've had several recommendation for [waterproof WS2812B strips](http://www.aliexpress.com/item/5-Meters-Individually-Addressable-Color-WS2812B-Waterproof-5050-SMD-RGB-WS2811-LED-Strip-White-PCB-60/1592816354.html)

Each strip has the following specs:

- $70 (including shipping)
- 300 LEDs
- 5 meters
- 120 degree emitting angle
- 5000 lumens
- 72 watts

If we get 35 of them, some napkin math would give us:

- 175 meters of strips
- 2520 watts
- 10,500 total LEDs
- 175,000 lumens (As bright as about 250 x 60W halogen bulbs)
- ~$2.5k

**"Stripeyness" Question**

With the current setup, we'd have

- ~7 wraps around the car (I'd estimate 25m of perimeter around the car)
- ~50cm between strips (car is ~3.5 meters tall)

If there are 50 cms between strips, how much distance do we need to place between our strips and the polycarbonate to prevent it from looking "stripey"?

See the [side view of the polycarbonate]("https://02337347925589272846.googlegroups.com/attach/60aa8062d575ed27/image%20(1).png?part=0.2&view=1&vt=ANaJVrFnE9LRHinrn2YPyG0IizoH2zhnGCRnwa9WVthJVIkFVWiOo2fa88zBys-kmq0OOha6R73fko4jDmnsCCGMBDtIHn5dX2ojwEnqtnGlZmFjxGc90iE") to clarify this question.

## Exterior LED Controllers

Fadecandy: https://github.com/scanlime/fadecandy

Purchasable on [Adafruit](http://www.adafruit.com/products/1689). Each one has the following specs:

- Runs 512 LEDs (8 strings of 64)
- $30 (including shipping)

If we get 20 of them we have:

- 10,240 total addressable LEDs
- 160 strips to connect
- $600

## USB hubs

Seems like we could use three. One for each side of the car and one in the center.

## USB cables

Standard cables should be fine, maximum length of 50ft

## Brain

We should bring an old macbook, which will let us debug things on the fly. If it breaks, it will be replaceable by other macbooks. Uses 45 watts

# Interior LEDs

TODO

# Sound System

TODO

# Generator

TODO
