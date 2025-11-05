# Le Page Turner

Simple two button bluetooth foot pedal for page turning while reading music off tablet, laptop, smartphone or ipad. The page turner connects to bluetooth enabled devices as an external keyboard, and sends "up"/"down" keystrokes when the primary push buttons are pressed.

## User instructions

### Bluetooth connection: new user

1. turn pedal on by sliding power switch "up"; micro-controller red LED flashes once.
2. clear all bluetooth profiles by pressing and holding "B" function button for more than 3 seconds.
3. scan for bluetooth devices on tablet/ipad and pair/connect to pedal.

The page turner pedal should connect with tablet/ipad as an external keyboard. Pressing primary left/right push buttons sends "up"/"down" keystrokes to tablet/ipad.

Once a connection is established, pairing with the same device should be automatic after turning the pedal on. Select page tuner on tablet/ipad if not.

The page turner will go into deep sleep after 3 hours of inactivity (and bluetooth connection will cease). In deep sleep, pushing primary push buttons should wake pedal up, and bluetooth connection should resume (perhaps with a delay of a few seconds). It is recommended to turn device off when not in use to conserve battery power.

If the bluetooth connection fails, either the wrong bluetooth profile has been selected (see below), or the maximum number of profiles has been reached. In the latter case, repeat step 2.

### Bluetooth connection: pairing with multiple devices

The pedal can pair with up to 3 devices (simultaneously). To connect to more than one device:

1. turn pedal on and connect to first device as usual.
1. press and release the "B" function button to cycle to second bluetooth profile and establish connection with second device.
1. press and release the "B" function button to cycle to third bluetooth profile and etablish connection with third device.

If connections were successful, tapping the "B" function button cycles through bluetooth profiles and activate one device at a time. 

After power on, the pedal will automatically connect to the last paired device. If connection with other devices fails, try tapping "B" function button to slowly cycle through profiles (using 5 second intervals to allow pairing).

The benefit of pairing with multiple devices is the "multi-mode" (see below) allowing to turn pages on several devices with a single push botton press. 

### Multi-mode

In normal mode, when the page turner is paired with multiple devices, it will only communicate with the current chosen bluetooth profile. Use "B" button to cycle through profiles (see above) to activate different device.

By tapping the "L" function button twice within 300ms, the page turner enters "multi-mode". In this mode, one press of the primary push buttons sends a keystroke to all paired devices, allowing the user to turn pages on multiple devices at a time. This feature allows players to display different pages on different devices but advance one page at a time through the music synchronously on all of them.

To disable "multi-mode" and return to normal mode, tap "L" function button twice within 300ms.

### Battery recharging 

Depending on the LiPo battery capacity, the page turner should be able to last for weeks on a single charge.

To recharge battery, attach USB-C cable to micro-controller (left side of pedal) and plug into laptop, PC or Mac computer USB port. Make sure the page turner is switch ON; the slide switch physically disconnects battery from micro-controller, so in order to recharge, the switch must be in "up" position.

**IMPORTANT: do not hook page turner pedal to a smartphone fast-charger! Only charge via computer.** LiPo batteries (and micro-controller circuit) require charging currents that are much lower than smartphone batteries. There is a danger that charging with fast-charger will damage LiPo battery.

A couple of tips for safe battery handling:

* LiPos tend to have life cycles of around 200-300 charges before becoming unstable
* Don't ever leave your LiPo in the Sun for too long; the extreme heat change can make your battery swell up and disfigure.
* Don’t leave LiPo battery fully charged for long (a day or so). It is best to use it "soon" and recharge when required.


## Components

### Electronics
* rechargeable 3.7V LiPo battery (recommended capacity 400-1000mAh)
* nice!nano pro micro with nRF52840 chip or [alternatives](https://github.com/joric/nrfmicro/wiki/ALternatives)
* 5x mini push button switch (6mm x 6mm)
* mini slide switch
* jumper wires (with female headers)
* 2-pin JST-PH connector 

### 3D printed
* pedal base
* pedal lid
* 2x mushroom shape push button
* 2x mushroom stems to connect with pedal lid
* piece to hold micro-controller in place
* 3x tiny rectangular prisms to hold function buttons in place
* tiny rectangular prism to hold slide switch in place

### Misc

* M3 x 10mm phillips screw 
* M3 nut
* Cat Tongue Grip Tape 2x107mm


## Building and wiring

1. press fit 2x primary push buttons (requires delicate force and/or minimal "bending")
1. press fit 3x function push buttons (requires delicate force and/or minimal filing/sanding slots down)
1. insert 3x rectangular prisms behind function buttons
1. insert slide switch on left panel 
1. insert rectangular prism to secure switch

Wiring is straightforward, see picture.
