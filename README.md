
![cmn](Pics/cmn.png)

**The Cheap Man's Node is the world most accessible Bitcoin Node, a do-it-yourself project targeting simplicity and efficacy at minimum costs.
A sleak 3D Printable and fully featured node built by the plebs, for the plebs.**

This FOSS project aims to create the world cheapest AND most reliable Bitcoin Node to lower the technical and economical barrier and reach true hyperbitcoinization.

Built around the Raspberry Pi 4, the most widespread device for self-made nodes, it significantly improve its reliability by addressing its downside in the most effective, yet economical, way possible.

You can make your own Cheap Man's Node by purchasing all the necessary components* listed below and 3D Print the files in this repo.
Alternately in the near future a pre-assembled version will be available for purchase.

![cmn](Pics/gif_pics_render.gif)

*unfortunately, some tiny bits of soldering is required


## Table of Contents

- [Feature Overview](#feature-overview)
- [Hardware](#hardware)
- [3D Printing](#3d-printing)
- [Soldering](#soldering)
- [Assembly](#assembly)
- [FAQ](#faq)
- [Contact](#contact)
- [License](#license)


## Feature Overview

- Powered by the Raspberry Pi 4, the most widespread device for self-made nodes
- GeekPi Aluminum Case, to maintain the CPU and other important components at safe temperature
- UPS with 2x18650 Li-Ion batteries, to maintain the device operational, even when your electric grid is not
- Interlocking assembly/disassembly system, no screws required.
- OS Agnostic. You are free to run your preferred OS
- Cheap AF, designed to be reliable without wasting precious sats on expensive hardware
- Low Profile: Its rather limited dimensions (150x80x50 mm) allow you to place it, or hide it, anywhere you want
- Completely FOSS: buy one or 3D print the case and build your own


 ## Hardware
      
**Buy a plug-n-play version:**
If you would like to support this project, a Geyser.fund link will be available to donate and/or purchase the Cheap Man's Node

**Build your own:**
Depending on what tool you have already available, it should cost you somewhere between 50 and 100 bucks excluding the RPi 4 and the SSD.

Tools needed:
- 3D Printer
- ~250g of PETG filament (PLA filament not recommended due to the temperature of the aluminum case)
- Soldering Iron
- Superglue

Hardware to buy:

| Parts                          | Quantity  | Link |
| ------------------------------ | --------- | ---- |
| Raspberry Pi 4 8GB             | 1  |[Amazon](https://www.amazon.com/Raspberry-Pi-Computer-Suitable-Workstation/dp/B0899VXM8F)  |
| SSD 1TB/2TB                    | 1  |[Amazon](https://www.amazon.com/Crucial-BX500-NAND-2-5-Inch-Internal/dp/B07YD579WM)       |
| Sabrent SSD-to-USB adapter     | 1  |[Amazon](https://www.amazon.com/Sabrent-2-5-Inch-Adapter-Optimized-EC-SSHD/dp/B011M8YACM) |
| USB to USB-C cable             | 1  |[AliExpress](https://www.aliexpress.com/item/1005004678079895.html) |
| JST Plug Connector Male+Female | 1  |[AliExpress](https://www.aliexpress.com/item/1005005334563700.html) |
| USB Type A Female              | 1  |[AliExpress](https://www.aliexpress.com/item/32834555144.html)      |
| Digital Voltmeter LED          | 1  |[AliExpress](https://www.aliexpress.com/item/1005003922909295.html) |
| Mini Push Button 6x6x16mm      | 1  |[AliExpress](https://www.aliexpress.com/item/4000420642261.html)    |
| AETHER 15W 3A UPS              | 1  |[AliExpress](https://www.aliexpress.com/item/1005002982442200.html) |
| 18650 Batteries                | 2  |[AliExpress 1](https://www.aliexpress.com/item/1005005363854781.html) or [AliExpress 2](https://www.aliexpress.com/item/1005005769176713.html) |
| USB 3.0 Extension Cable S3A-S4B 10cm | 1  |[AliExpress](https://www.aliexpress.com/item/1005003527380361.html) |
| Aluminum Case for RPi 4 (No-FAN) | 1  |[AliExpress](https://www.aliexpress.com/item/4001365568030.html) or [PiHut](https://thepihut.com/products/aluminium-armour-heatsink-case-for-raspberry-pi-4)
| Dupont Wires M-F               | 1  |[AliExpress](https://www.aliexpress.com/item/3256805759353801.html) |
| Heat shrink tube kit           | 1  |[AliExpress](https://www.aliexpress.com/item/4000971878875.html) |
| 20 AWG Wires or lower          | 1  |Use what you have at home |


## 3D Printing

All parts have been processed with PrusaSlicer and printed in Petg on a cheap 3D Printer. Everything can and should be printed without supports.

Petg is the recommended filament as it withstand the heat better than Pla and warp less than Abs, but with that being said, feel free to 3D print it in the material you believe to be more adequate and don't esitate to send me your feedbacks once you test it.

![cmn](Pics/gif_3dprinting.gif)

3D printing details:

| Setting | Value |
| --- | --- |
| Material | Petg |
| Nozzle tempertature | 230°C |
| Print bed tempertature | 80°C |
| Layer height | 0.12mm |
| Perimeters | 2 |
| Infill | 30% |
| Pattern | Rectilinear |
| Avoid crossing perimeters | On (avoid hairy print with Petg) |
| Solid infill threshold area | 5mm² |
| Skirt | On |


Part specific details:

| Part File | Additional Instructions | Count | Photo |
|-----------|-------------------------|-------|-------|
| [1_top_A](STL%20Files/1_top_A.stl) OR [1_top_B](STL%20Files/1_top_B.stl) <br>More details [HERE](Pics/top_a_or_b.jpg) | Infill: 40% <br>Solid infill threshold area: 30mm² <br>Setting for Height ranges: Start at height: 2.4 > Perimeters: 3 | 1 | ![A](Pics/3dprinting/3dprinting-part-01.png) |
| [2_disk_usb_top](STL%20Files/2_disk_usb_top.stl) AND [2_disk_usb_bottom](STL%20Files/2_disk_usb_bottom.stl)  |  | 2 | ![B](Pics/3dprinting/3dprinting-part-02.png) |
| [3_disk_usb_holder](STL%20Files/3_disk_usb_holder.stl) | Perimeters: 3 | 1 | ![C](Pics/3dprinting/3dprinting-part-03.png) |
| [4_rpi_holder_body](STL%20Files/4_rpi_holder_body.stl) | Detect thin walls: Off | 1 | ![D](Pics/3dprinting/3dprinting-part-04.png) |
| [5_ups_base](STL%20Files/5_ups_base.stl) | Detect thin walls: Off | 1 | ![D](Pics/3dprinting/3dprinting-part-05.png) |
| [6_front_holder](STL%20Files/6_front_holder.stl) | Detect thin walls: Off | 1 | ![D](Pics/3dprinting/3dprinting-part-06.png) |
| [7_locking](STL%20Files/7_locking.stl) | Solid infill threshold area: 8mm² <br>Detect thin walls: Off | 1 | ![D](Pics/3dprinting/3dprinting-part-07.png) |
| [8_ups_box](STL%20Files/8_ups_box.stl) |  | 1 | ![D](Pics/3dprinting/3dprinting-part-08.png) |
| [9_ups_cable_holder](STL%20Files/9_ups_cable_holder.stl) | Perimeters: 3 <br>Detect thin walls: Off | 1 | ![D](Pics/3dprinting/3dprinting-part-09.png) |
| [10_enclosure](STL%20Files/10_enclosure.stl) | Fill density: 20% <br>Layer height: 0.2mm <br>Detect thin walls: Off | 1 | ![D](Pics/3dprinting/3dprinting-part-10.png) |
| [11_back_holder](STL%20Files/11_back_holder.stl) |  | 1 | ![D](Pics/3dprinting/3dprinting-part-11.png) |
| [12_part_holder](STL%20Files/12_part_holder.stl) | Fill density: 50% <br>Variable layer height: On (manually reduce the height down to 0.08mm in the lower parts of the sliding rails to avoid Overhanging perimeters that would otherwise hinder the drawer movement) | 1 | ![D](Pics/3dprinting/3dprinting-part-12.png) |
| [13_box_foot](STL%20Files/13_box_foot.stl) | Material: TPU <br>Print Speed must be significantly decreased to print in this material | 4 | ![D](Pics/3dprinting/3dprinting-part-13.png) |
| [14_usb_cover](STL%20Files/14_usb_cover.stl) | Perimeters: 4 <br>Detect thin walls: Off <br>Variable layer height: On (manually reduce the height down to 0.08mm near the top and bottom to avoid Overhanging perimeters that would otherwise impact the cosmetic function of the part) | 1 | ![D](Pics/3dprinting/3dprinting-part-14.png) |




## Soldering

01 - Cut the M-JST connector wires to reach a length of 55mm
![cmn](Pics/Soldering/soldering-01.jpg)

02 - Leave the F-JST connector wires at the length of 105mm (if longer, cut it down to 105mm)
![cmn](Pics/Soldering/soldering-02.jpg)

03 - Solder the Red and Black wires to the USB-F*, apply Heat Shrink Tube then cut the wires to reach a length of 100mm
![cmn](Pics/Soldering/soldering-03.jpg)
*when soldering the two wires, compare the seam of the USB-F shield depicted above to make sure that the orientation is correct

04 - Cut the Red and Black M-Dupont connector wires to reach a length of 60mm
![cmn](Pics/Soldering/soldering-04.jpg)

05 - Cut the Red F-Dupont connector wire to reach a length of 50mm
![cmn](Pics/Soldering/soldering-05.jpg)

06 - Cut another Red F-Dupont connector wire to reach a length of 85mm
![cmn](Pics/Soldering/soldering-06.jpg)

07 - Cut the Red wire of the Digital Voltmeter to reach a length of 50mm
![cmn](Pics/Soldering/soldering-07.jpg)

08 - Cut the Black wire of the Digital Voltmeter to reach a length of 100mm
![cmn](Pics/Soldering/soldering-08.jpg)

09 - Solder the 60mm Black M-Dupont connector wire and the 50mm Red F-Dupont connector wire to the Mini Push Button, apply Heat Shrink Tube
![cmn](Pics/Soldering/soldering-09.jpg)

10 - Solder the 60mm Red M-Dupont connector wire to the Digital Voltmeter Red wire, apply Heat Shrink Tube
![cmn](Pics/Soldering/soldering-10.jpg)

11 - Solder the 85mm Red F-Dupont connector wire to the M-JST connector Red wire, apply Heat Shrink Tube
![cmn](Pics/Soldering/soldering-11.jpg)

12 - Solder the M-JST connector Black wire to the Digital Voltmeter Black wire, apply Heat Shrink Tube
![cmn](Pics/Soldering/soldering-12.jpg)

13 - Insert the Dupont connectors as depicted
![cmn](Pics/Soldering/soldering-13.jpg)

14 - Insert the Mini Push Button and the Digital Voltmeter to the 3D printed 6_front_holder as depicted, then use a tiny drop of superglue* to secure them in place
![cmn](Pics/Soldering/soldering-14.jpg)
*make sure that the superglue does not flow inside the Mini Push Button mechanism, holding the piece sideways is recommended to avoid it

15 - Solder the F-JST connector wires to the UPS board as depicted
![cmn](Pics/Soldering/soldering-15.jpg)

16 - Solder the USB-F Red and Black wires to the UPS board as depicted, again making sure that the USB-F orientation is correct
![cmn](Pics/Soldering/soldering-16.jpg)




## Assembly

01 - Mount the Aluminum Case on the Raspberry Pi and fit 1_top on it
<p float="left">
  <img src="Pics/Assembly/assembly-01.jpg" width="49.5%" />
  <img src="Pics/Assembly/assembly-02.jpg" width="49.5%" />
</p>

02 - Carefully connect 3_disk_usb_holder and 4_rpi_holder_body together
<p float="left">
  <img src="Pics/Assembly/assembly-03.jpg" width="49.5%" />
  <img src="Pics/Assembly/assembly-04.jpg" width="49.5%" />
</p>

03 - Fit the pieces together by connecting the hooks
<p float="left">
  <img src="Pics/Assembly/assembly-05.jpg" width="49.5%" />
</p>

04 - Fix the 2_disk_usb_top AND 2_disk_usb_bottom components around the female USB socket of the USB 3.0 Extension Cable 
<p float="left">
  <img src="Pics/Assembly/assembly-06.jpg" width="49.5%" />
  <img src="Pics/Assembly/assembly-07.jpg" width="49.5%" />
</p>
  
05 - Insert the two 18650 batteries in the UPS and snap it into the 5_ups_base as shown below. Make sure that the batteries are mounted in parallel
<p float="left">
  <img src="Pics/Assembly/assembly-08.jpg" width="49.5%" />
  <img src="Pics/Assembly/assembly-09.jpg" width="49.5%" />
</p>

06 - Slide the 6_front_holder and the Voltmeter previously glued to it into the 5_ups_base
<p float="left">
  <img src="Pics/Assembly/assembly-10.jpg" width="49.5%" />
  <img src="Pics/Assembly/assembly-11.jpg" width="49.5%" />
</p>

07 - Slowly and carefully insert at an angle the UPS female USB in the 7_locking component, as demonstrated in the picture
<p float="left">
  <img src="Pics/Assembly/assembly-12.jpg" width="49.5%" />
  <img src="Pics/Assembly/assembly-13.jpg" width="49.5%" />
</p>

08 - Gently push the 7_locking part down into the 6_front_holder without putting too much pressure. If you encounter some resistance, slowly scrape the connecting part with sandpaper.
<p float="left">
  <img src="Pics/Assembly/assembly-14.jpg" width="49.5%" />
  <img src="Pics/Assembly/assembly-15.jpg" width="49.5%" />
</p>

09 - Pass the Male JST Plug through the appropriate hole in the 5_ups_base component, then connect it to the Female JST Plug on the UPS
<p float="left">
  <img src="Pics/Assembly/assembly-16.jpg" width="49.5%" />
  <img src="Pics/Assembly/assembly-17.jpg" width="49.5%" />
</p>

10 - Test the Voltmeter by pressing the button. If everything is done correctly, it will show you the voltage of the batteries
<p float="left">
  <img src="Pics/Assembly/assembly-18.jpg" width="49.5%" />
</p>

11 - Place the Voltmeter cable in the 9_ups_cable_holder, then fit it to the 5_ups_base by connecting the hooks
<p float="left">
  <img src="Pics/Assembly/assembly-19.jpg" width="49.5%" />
  <img src="Pics/Assembly/assembly-20.jpg" width="49.5%" />
</p>

12 - Vertically snap the 8_ups_box to the 5_ups_base and the 2_disk_usb to the 4_rpi_holder_body
<p float="left">
  <img src="Pics/Assembly/assembly-21.jpg" width="49.5%" />
  <img src="Pics/Assembly/assembly-22.jpg" width="49.5%" />
</p>

13 - Moving on to the 10_enclosure, let's start by supergluing the 4x 13_box_foot to it
<p float="left">
  <img src="Pics/Assembly/assembly-23.jpg" width="49.5%" />
</p>
<p float="left">
  <img src="Pics/Assembly/assembly-24.jpg" width="49.5%" />
  <img src="Pics/Assembly/assembly-25.jpg" width="49.5%" />
</p>

14 - Slide the Raspberry Pi and the 3D printed components attached to it 9/10th of the way in the 10_enclosure rails. Carefully push the male USB of the USB 3.0 Extension Cable through the appropriate opening, rotating it 90 degrees and inserting it from top to bottom. Once done, push it all the way in and insert the male USB into the Raspberry Pi
<p float="left">
  <img src="Pics/Assembly/assembly-26.jpg" width="49.5%" />
  <img src="Pics/Assembly/assembly-27.jpg" width="49.5%" />
  <img src="Pics/Assembly/assembly-28.jpg" width="49.5%" />
  <img src="Pics/Assembly/assembly-29.jpg" width="49.5%" />
</p>

15 - Slide the 5_ups_base and all of the components attached to it all the way in the 10_enclosure rails, gently pushing the voltmeter and the voltmeter button through the appropriate openings
<p float="left">
  <img src="Pics/Assembly/assembly-30.jpg" width="49.5%" />
  <img src="Pics/Assembly/assembly-31.jpg" width="49.5%" />
</p>

16 - Connect the Sabrent adapter to the SSD, then tie the cable as shown in the picture and slide it all the way in the 10_enclosure rails
<p float="left">
  <img src="Pics/Assembly/assembly-32.jpg" width="49.5%" />
  <img src="Pics/Assembly/assembly-33.jpg" width="49.5%" />
</p>

17 - Connect the male USB of the Sabrent adapter to the female USB of the Extension Cable, then slide the 12_part_holder component in the 10_enclosure rails
<p float="left">
  <img src="Pics/Assembly/assembly-34.jpg" width="49.5%" />
  <img src="Pics/Assembly/assembly-35.jpg" width="49.5%" />
</p>

18 - To keep the device tightly closed, use two well-stretched elastic bands mounted in an X shape, as shown in the photo
<p float="left">
  <img src="Pics/Assembly/assembly-36.jpg" width="49.5%" />
  <img src="Pics/Assembly/assembly-37.jpg" width="49.5%" />
</p>

19 - Vertically slide the 11_back_holder into the 10_enclosure
<p float="left">
  <img src="Pics/Assembly/assembly-38.jpg" width="49.5%" />
  <img src="Pics/Assembly/assembly-39.jpg" width="49.5%" />
</p>

20 - Finally, connect the Raspberry Pi and the UPS with the USB to USB-C cable and connect the UPS to a 5V charger with a USB-C cable you have around. Note that, on average, the device will drain slightly more than 1A, so it's recommended to use a charger that can supply at least 1.5A or 2A
<p float="left">
  <img src="Pics/Assembly/assembly-40.jpg" width="49.5%" />
</p>

## FAQ

* **Why the Raspberry?**

    Besides being cheap, It have some advantage compared to other alternatives.
Unlike common laptops, it consumes very little energy, saving you hundreds of thousands of sats every year on your energy bill.
Also, being one of the most common hardware used for Bitcoin nodes, it has plenty of guides and huge communities to support you in case of need.

* **But Doesn't it have some reliability issue?**

    There are some misconception surrounding the reliability of the Raspberry's for this kind of use.
First note that, being one of the most common hardware used for Bitcoin Nodes, it's quite natural that the most common problems discussed online are about them.
The most common and widespread issue involving them are mainly of two type:

  **Overheating** - A terminal hardware issue often involves overheating, but in the case of the Raspberry Pi 4 the problem arises with the ram. Most of the Cooling system for the RPI4, whether are embedded in a case or not, dissipate the heat generated by the CPU, but often avoid dissipating the heat generated by the Ram, which occasionally lead to a permanent damage
By using a well-engineered cooling system that effectively cools down the main Raspberry Pi components, such as the Armor Case used in the Cheap Man's Node, the risk of encountering such issue would be avoided.

    **Power outage** - Sudden and Unexpected power outage or power spike can permanently damage the Raspberry and/or the content being written on the disk, forcing you to redo everything from skratch, once again. The usage of the UPS will guarantee you not only an impeccable uptime but also avoid the consequence of a blackout.

* **Can I use the UPS for other stuff?**

    Absolutely, the UPS is rated to constantly output up to 5A at 5 Volt, so you can connect other devices along the Raspberry, like a low power Router, to ensure you are always connected even during power outage. This is also the reason why the USB cable is placed on the outer part of the Node instead of being hidden inside.

* **Can I buy a pre-assembed Node from you?**

    Not yet, once it becomes available for purchase I'll provide a link for it in this page.

* **What is the recommended 3D printer for this project?**

    Any printer will do the job! Tolerances are quite generous and, depending the dimension of the part, are between 0.2 and 0.4 millimiters.
A standard plate of 220x220 will allow you to print all the components, except 10_Enclosure, in one session.

## Contact
You can reach out on [Twitter](https://twitter.com/CheapMansNode) or contact me at: cheapmansnode at protonmail dot com

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
