# The-Robot-Trick-Dog

An all mechanical, RX controlled mini robot trick dog whose main purpose is to let u control it with a transmitter and see what cool tricks u can make it do. Its purpose isn't to walk in a straight line since that would require code and it wouldn't be fully mechanical anymore.

## BOM (Bill of Materials)

| Product | Qty | Cost (USD) | Link |
|---|---:|---:|---|
| Foam Board | 1 | $6.81 | [Link](https://www.vortex-rc.com/product/fliteboard-500x200mm-10-sheet-pack/) |
| Micro Servo Motors and Servo Horns | 4 | $4.32 | [Link](https://robocraze.com/products/sg90-micro-servo-motor) |
| RC Receiver and Transmitter | 1 | $36.12 | [Link](https://robu.in/product/flysky-fs-i4x-2-4ghz-4ch-afhds-r-c-transmitter-fs-a6-receiver/) |
| Y Servo Connectors | 2 | $1.36 | [Link](https://robu.in/product/1jr-male-2-futaba-female-y-type-servo-extension-wire300mm/) |
| Electrical Tape | 1 | $1.47 | [Link](https://robu.in/product/multicomp-pro-mp002145-tape-pvc-19mm-x-8m-red/) |
| Double-Sided Foam Tape | 1 | $0.23 | [Link](https://onlyscrews.in/products/double-side-foam-tape-22mm-x-2-5meters) |
| Hot Glue | 1 | $1.48 | [Link](https://www.amazon.in/MGR-Melt-Plastic-Small-Black/dp/B07N1TMTF2) |
| LiPo Battery | 1 | $18.40 | [Link](http://robu.in/product/orange-2200mah-3s-30c60c-lithium-polymer-battery-pack-lipo/) |
| ESC with Built-in BEC | 1 | $3.42 | [Link](https://robu.in/product/30a-bldc-esc-electronic-speed-controller/) |

**Total Estimated Cost: $87.93**

## My build process and how u can replicate it

## 1. Make the body and legs

I used some scrap foam board left over from my Flite Test P-51 Mustang build. I originally planned to make a flat body but then decided to use some folding techniques I learned while building my RC plane. I marked out the body, cut it out, folded the sections upwards and used hot glue to hold everything together.

For the legs I cut out four more pieces of foam board and wrapped them in electrical tape for extra grip and strenght.

<p>
<img src="https://cdn.hackclub.com/01a00b0a-aef0-7a0c-a10a-67c4e8709437/image.png" alt="Body template" width="25%">
<img src="https://cdn.hackclub.com/01a00b0b-64d7-71f7-a375-9158c1d73e61/image.png" alt="Folded body" width="25%">
</p>

<p>
<img src="https://cdn.hackclub.com/01a00b0c-db4e-72d7-b759-e4e29a855905/image.png" alt="Robot legs" width="25%">
<img src="https://cdn.hackclub.com/01a00b0c-f2c0-7942-9159-4c543aa1e151/image.png" alt="Legs" width="25%">
</p>

## 2. Attach the servos

For the servos I reused the ones from my first RC plane. That plane had been through a LOT of crashes so I wasn't really going to use those servos for flying again anyway. I glued the legs directly onto the servo horns.

Before mounting the servos I covered the body with duct tape so I could remove them later without ripping the paper off the foam board. I ran out of hot glue sticks so I used double-sided foam tape instead and honestly it worked suprisingly well.

<p>
<img src="https://cdn.hackclub.com/01a00b0e-3a7d-7e3f-91bd-f16ba7349360/image.png" alt="Servo and leg" width="25%">
<img src="https://cdn.hackclub.com/01a00b45-a0f9-71a7-a695-699e6986d16b/image.png" alt="Attached legs" width="25%">
</p>

<p>
<img src="https://cdn.hackclub.com/01a00b48-3ba5-7e94-a4e7-57f414380b9b/image.png" alt="Servo mounting" width="25%">
<img src="https://cdn.hackclub.com/01a00b48-5243-7786-b8e4-9ec2752135bb/image.png" alt="Mounted servos" width="25%">
</p>

## 3. Connect the diagonal servos

Instead of controlling all four servos individually I connected the diagonal servos using Y servo cables. This makes the setup much simpler.

- Servo 1 + Servo 4 → Y cable → CH1
- Servo 2 + Servo 3 → Y cable → CH2

The servos on each diagonal need to move in opposite directions so when one leg moves one way the diagonal leg moves the other way. I forgot to take a photo of the actual Y connectors so the diagram shows the basic idea.

<p>
<img src="https://cdn.hackclub.com/01a00b4d-4788-70c8-97d0-586b3336caed/image.png" alt="Servo wiring diagram" width="25%">
<img src="https://cdn.hackclub.com/01a00b58-e4e6-7f0f-8a30-1c3f7306baaf/image.png" alt="Receiver wiring" width="25%">
</p>

## 4. Clean up the wires

The servo wires were around 6 to 7 inches long. Instead of cutting them I just looped the excess wire and secured it to the body. It isn't exactly the cleanest wiring ever but it works. Just make sure the wires stay away from the servo horns and legs.

<p>
<img src="https://cdn.hackclub.com/01a00b4d-90ec-72be-bebe-d99e97c7b2fb/image.png" alt="Wire management" width="25%">
<img src="https://cdn.hackclub.com/01a00b4d-b05f-77c0-adba-6cc568e3b255/image.png" alt="More wire management" width="25%">
</p>

## 5. Power the robot

Four servos can draw a suprising amount of current. I first tried using a small 3.7V battery but it wasn't able to provide what I needed. I ended up using the setup I already had available:

- 2200 mAh 3S 11.1V 30C LiPo
- ESC with an integrated BEC
- Servo extension cable
- RC receiver

The ESC's BEC provides power to the receiver and servos from the LiPo. Make sure the BEC output voltage is suitable for your receiver and servos. Never connect the battery directly to them unless the voltage is within their rated range.

## 6. Keep the big battery off the robot

I didn't put the battery and ESC directly on the robot because the battery is heavy compared to the body, the servos aren't powerful enough to move that much weight and the battery is actually longer than the robot itself.

Since this robot is mainly meant to do tricks in a small area rather than walk around a room, I just kept the battery off the robot and used an extension cable to give it some freedom to move. A smaller battery and suitable power setup could potentially let u fit everything directly on the robot.

## 7. Test the movement

Once everything is connected, turn on the transmitter and receiver and test each movement slowly. Check that:

- All four servos move in the correct direction.
- The diagonal servos move opposite to each other.
- The legs don't hit the body.
- The servo horns don't collide with anything.
- The wires stay away from moving parts.
- The robot stays reasonably balanced.

If a servo moves the wrong way u may need to reverse that channel on your transmitter or change how the servo is mounted.

## 8. Start experimenting with tricks

Once the basic movement works u can start messing around with the transmitter controls. Because the robot only has two controlled servo groups u can get some pretty interesting movements without needing a microcontroller.

The whole point of this project is to experiment and see what weird tricks u can make it do!
