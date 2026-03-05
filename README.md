# Samus Cyberdeck

I want to gut one of my Chromebook Pixel 2015s (codename Samus) and make something like this with it: https://www.youtube.com/watch?v=eR3kf-nUY-s

## Requirements and compromises

- Keep the lightbar, including tap for battery level functionality
- Expose at least these external ports: two USB-C, two USB-A
    - Nice to have: SD card reader, headset jack
- Speakers not required

## BoM

### Display

BOE 12.6inch NV126B5M-N41 1920x515 LCD

- Has separate touch connector and interface board from eDP, it does not go through the eDP connector.
- eDP is a 40 pin two lane connector but the touch part is unused.

## Links/resources

- Display used in linked video: VSDISPLAY 12.6" NV126B5M-N41 12.6inch1920X515 LCD Screen Work with 2 HD-MI Mini LCD Controller VS-RTD2556HM-V1, Work with Raspberry Pi: https://www.amazon.com.au/VSDISPLAY-NV126B5M-N41-12-6inch1920X515-Controller-VS-RTD2556HM-V1/dp/B08FJ33247
    - https://www.panelook.com/NV126B5M-N41_BOE_12.6_LCM_parameter_44187.html
- Keyboard used in linked video: https://iqunix.store/products/iqunix-og80-wormhole-wireless-mechanical-keyboard?variant=39828939898940
    - Apparently hard to disassemble and not recommended.
- Similar projects:
    - https://www.reddit.com/r/MechanicalKeyboards/comments/qjfslc/designed_and_printed_a_mini_ultrawide_display/

### Display

- The three types of common eDP pinout: https://hackaday.io/project/179868-all-about-laptop-display-reuse/log/209701-common-edp-laptop-panel-pinouts
    - 30 pin two lane (eDP 1.2)
    - 40 pin two lane (eDP 1.2) with touch (possibly via USB or someother protocol with clock and data and interrupt pins)
    - 40 pin four lane (eDP 1.4), no touch
- A successful attempt at an adapter from 40 pin four lane from computer to 30 pin two lane display: https://community.frame.work/t/40pin-edp-framework-4lane-to-30pin-edp-2-lane/38745
- A different attempt with some pictures and possibly useful information: https://flogbook.wordpress.com/2018/09/30/passive-displayport-to-edp-adapter/
