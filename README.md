### **Starbie**
I'm making a Starbie, in the shape of the soul from Undertale. Please note that there are two files directly imported from KiCad which are the Schematics and PCB, the gerber files are listed seperately. There's each of them individually, and one gerbers.zip file.

Here's a picture of it:
<img width="1919" height="1004" alt="Screenshot 2026-10-11 181855" src="https://github.com/user-attachments/assets/c3c9a7c7-63da-4f80-88fd-146794068089" />
<img width="1918" height="1031" alt="Screenshot 2026-10-20 194448" src="https://github.com/user-attachments/assets/e5480625-9a34-4ca8-824c-321c8b82e3a0" />

### **Here's what some of the buttons do!**

1. Button One (BUTTON_ONE_PIN/XIAO D2 in the Arduino code):
   - Normal View: Opens the radial menu
   - Menu View: Confirms/selects the currently highlighted menu action
2. Button Two (BUTTON_TWO_PIN/XIAO D3):
   - Toggles the stats screen on and off, + it shows Joy, Energy, Fullness, Temperature, and Humidity
     *Does not change pet's stats directly, simply lets you check on them

### **Here's the motion controls!**
  
1. Tilt -- inside radial menu
   - Firstly press button one to open the menu, the board acts like an "air mouse," and tilting the board moves a ball across the screen into one of four diagonal sectors to choose an action:
   - Top/Nap: Sleeps, increases NRG, emits Z's
   - Right/Play: Runs two fast laps, increases joy, lowers NRG
   - Bottom/Feed: Wiggles and jumps, increases fullness
   - Left/Pet: Jumps and emits hearts, increases joy
2. Shake/Normal View
   - Shake the heart a bit, and wake up your sleeping pet! *small boost to joy, small decrease to NRG + fullness
  
### **!!IMPORTANT FOR BILL OF MATERIALS!!
In Halflife I was told to add all the materials I would be using including anything I already own at $0, but Halflife requires everything added to be a minimum of $0.01 so everything listed to be $0.01 are things I already have!! Look at the BOM below for instructions for the custom PCB, the rest is basically a repeat of what's written in the Halflife BOM. FOR THE CUSTOM STARBIE PCB PLEASE CHANGE SHIPPING TO GLOBAL STANDARD DIRECT LINE AND CHANGE THE SURFACE FINISH FROM Hasl (with lead) TO LeadFree HASL.**


### **Starbie Project Bill of Materials (BOM)**

| Part / Description | Qty | Unit Price | Total Price | Vendor | Link |
| --- | --- | --- | --- | --- | --- |
| **Custom Starbie PCB** (Fabricated circuit board) | 1 | $4.00 | $4.00 | JLCPCB | https://cart.jlcpcb.com/quote?stencilLayer=2&stencilWidth=100&stencilLength=100&stencilCounts=5&plateType=1&spm=Jlcpcb.Homepage.1010
| **Seeed Studio XIAO ESP32C3** (Main microcontroller) | 1 | [blank] | [blank] | [blank] | [blank] |
| **0.96" I2C OLED Display (SSD1306)** (Screen for animations) | 1 | [blank] | [blank] | [blank] | [blank] |
| **MPU6050 Module** (6-axis accelerometer/gyroscope) | 1 | [blank] | [blank] | [blank] | [blank] |
| **DHT Sensor** (Temperature & humidity sensor) | 1 | [blank] | [blank] | [blank] | [blank] |
| **Mini Pushbutton Switches** | 2 | [blank] | [blank] | [blank] | [blank] |
| **Male Breakable Pin Headers** | 1 | [blank] | [blank] | [blank] | [blank] |
| **Female Breakable Pin Headers** (Socket strip) | 1 | [blank] | [blank] | [blank] | [blank] |
| **USB-C Data Cable** | 1 | [blank] | [blank] | [blank] | [blank] |

* **Total Tax & Shipping for the whole order:** [blank]

---


   - *Make sure to change shipping to Global Standard Direct Line
   - *Make sure to change the Surface Finish from HASL (with lead) to LeadFree HASL

Things I already have/I'm buying myself:

5. Momentary PushButton Switch - 12mm Square x1
6. 20 Pcs 10 Pairs 40 Pin 1x40 Single Row Male And Female 2.54 Breakable Pin Header PCB JST Connector Strip For Arduino DIY x1
7. ZeroneTeck USB C Data Cable
   
  


