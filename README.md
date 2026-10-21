# Starbie
I'm making a Starbie, in the shape of the soul from Undertale. Please note that there are two files directly imported from KiCad which are the Schematics and PCB, the gerber files are listed seperately. There's each of them individually, and one gerbers.zip file.

Here's a picture of it:
<img width="1919" height="1004" alt="Screenshot 2026-10-11 181855" src="https://github.com/user-attachments/assets/c3c9a7c7-63da-4f80-88fd-146794068089" />

Here's what some of the buttons do! 

1. Button One (BUTTON_ONE_PIN/XIAO D2 in the Arduino code):
   - Normal View: Opens the radial menu
   - Menu View: Confirms/selects the currently highlighted menu action
2. Button Two (BUTTON_TWO_PIN/XIAO D3):
   - Toggles the stats screen on and off, + it shows Joy, Energy, Fullness, Temperature, and Humidity
     *Does not change pet's stats directly, simply lets you check on them

Here's the motion controls!
  
1. Tilt -- inside radial menu
   - Firstly press button one to open the menu, the board acts like an "air mouse," and tilting the board moves a ball across the screen into one of four diagonal sectors to choose an action:
   - Top/Nap: Sleeps, increases NRG, emits Z's
   - Right/Play: Runs two fast laps, increases joy, lowers NRG
   - Bottom/Feed: Wiggles and jumps, increases fullness
   - Left/Pet: Jumps and emits hearts, increases joy
2. Shake/Normal View
   - Shake the heart a bit, and wake up your sleeping pet! *small boost to joy, small decrease to NRG + fullness
  
BOM (Bill of Materials) Table:
1. Custom Starbie PCB (Fabricated cirbuit board from Gerber Files) x1
   - Price: $8.16
   - Vendor: JLCPCB -- https://jlcpcb.com/?from=VGSU&utm_source=google&utm_medium=cpc&utm_campaign=14179457750&gad_source=1&gad_campaignid=14179457750&gbraid=0AAAAABS1QqmjhvpyM6UansMwKMCcapsDe&gclid=CjwKCAjwotzWBhBFEiwA1JhPoJelGj7nkAeiYrvhPq2GhTAk_WHOOXMeSoFLwSAmz8AfTMGFaQEYhRoCad8QAvD_BwE
   - *Make sure to change shipping to Global Standard Direct Line
   - *Make sure to change the Surface Finish from HASL (with lead) to LeadFree HASL
2. 
  


