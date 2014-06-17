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

# Exterior LEDs

The current plan would have the following specs

- ~175,000 lumens
- ~2600 watts
- ~$3k

## LED strips
I've had several recommendation for [waterproof WS2812B strips](http://www.aliexpress.com/item/100M-20x-5m-30leds-M-WS2812B-36W-5050-LEDs-Digital-LED-Strip-WS2812B-M-IP65-DC5V/1396783184.html)

Each strip has the following specs:

- $0.20 per LED (plus shipping)
- 6k LEDs per strip
- 200m
- 120 degree emitting angle
- ~100,000 lumens (17 lumens/led)
- 1440 watts (7.2 watts/m)

If we get 2 of them, some napkin math would give us:

- 400 meters of strips
- 2880 watts
- 12,000 total LEDs
- 200,000 lumens (As bright as about 300 x 60W halogen bulbs)
- ~$2.5k

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
