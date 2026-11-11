### **Starbie**
I'm making a Starbie, in the shape of the soul from Undertale. Please note that there are two files directly imported from KiCad which are the Schematics and PCB, the gerber files are listed seperately. There's each of them individually, and one gerbers.zip file.

Here's a picture of it:
<img width="1919" height="1032" alt="Screenshot 2026-11-11 065542" src="https://github.com/user-attachments/assets/8fa29fd8-8820-4235-a6d3-0e1e290a5b2a" />
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
| **Seeed Studio XIAO ESP32C3** (Main microcontroller) | 1 | $5.49 | $5.49 | OpenElab Inc. | https://shop.com/products/15171276669252?variantId=55134673404228&utm_source=google_display&utm_medium=&utm_campaign=24249207249&utm_content=824789162836&adgroup=201840906844&gclid=CjwKCAjwotzWBhBFEiwA1JhPoHlxAZ9mIDQ_HcftdG87PVtMWQWhvZ1NPeqvN5uGyvO27BO0uU62zBoCbrsQAvD_BwE&gad_source=1&gad_campaignid=24249207249&gbraid=0AAAAA9hdXieHU29oAyEHINvF9mm5ITR3N |
| **0.96" I2C OLED Display (SSD1306)** (Screen for animations) | 1 | $1.02 | $1.02 | AliExpress | https://www.aliexpress.us/item/3256808426200900.html?src=google&src=google&albch=shopping&acnt=708-803-3821&isdl=y&slnk=&plac=&mtctp=&albbt=Google_7_shopping&aff_platform=google&aff_short_key=UneMJZVf&gclsrc=aw.ds&albagn=888888&ds_e_adid=&ds_e_matchtype=&ds_e_device=c&ds_e_network=x&ds_e_product_group_id=&ds_e_product_id=en3256808426200900&ds_e_product_merchant_id=5480922393&ds_e_product_country=US&ds_e_product_language=en&ds_e_product_channel=online&ds_e_product_store_id=&ds_url_v=2&albcp=19558607238&albag=&isSmbAutoCall=false&needSmbHouyi=false&gad_source=1&gad_campaignid=19566915268&gbraid=0AAAAAD6I-hFRHflJGCWNZNxA3pS6luCfe&gclid=CjwKCAjwotzWBhBFEiwA1JhPoCZgiQ26CRvcJ1qDZ60ryEK_80BIlHI656g-7cJhP5qdBNJaf_03VRoCZvgQAvD_BwE&gatewayAdapt=glo2usa |
| **MPU6050 Module** (6-axis accelerometer/gyroscope) | 1 | $1.09 | $1.09 | AliExpress | https://www.aliexpress.us/item/3256810415729295.html?spm=a2g0o.productlist.main.2.429f4881VWTRpP&algo_pvid=6fff6680-c85b-4aef-94f2-83463e1b110b&algo_exp_id=6fff6680-c85b-4aef-94f2-83463e1b110b-1&pdp_ext_f=%7B%22order%22%3A%22927%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&pdp_npi=6%40dis%21USD%212.43%211.09%21%21%2116.16%217.26%21%40210328c017944095934673565e10bb%2112000052945138544%21sea%21US%210%21ABX%211%210%21n_tag%3A-29910%3Bd%3A8a6c86e2%3Bm03_new_user%3A-29895%3BpisId%3A5000000218165391&curPageLogUid=c3nIiG7YoFHd&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005010602044047%7C_p_origin_prod%3A |
| **DHT11 Sensor** (Temperature & humidity sensor) | 1 | $0.00 | $0.00 | AliExpress | https://www.aliexpress.us/item/2251832654578110.html?src=google&src=google&albch=shopping&acnt=708-803-3821&isdl=y&slnk=&plac=&mtctp=&albbt=Google_7_shopping&aff_platform=google&aff_short_key=UneMJZVf&gclsrc=aw.ds&albagn=888888&ds_e_adid=&ds_e_matchtype=&ds_e_device=c&ds_e_network=x&ds_e_product_group_id=&ds_e_product_id=en2251832654578110&ds_e_product_merchant_id=100990838&ds_e_product_country=US&ds_e_product_language=en&ds_e_product_channel=online&ds_e_product_store_id=&ds_url_v=2&albcp=19558607238&albag=&isSmbAutoCall=false&needSmbHouyi=false&gad_source=1&gad_campaignid=19566915268&gbraid=0AAAAAD6I-hFRHflJGCWNZNxA3pS6luCfe&gclid=CjwKCAjwotzWBhBFEiwA1JhPoPFifqgQYVMZr4quX26TGl3DfBxFLOo6ubxXwE4JU9EE23WffCHeJRoCIasQAvD_BwE&gatewayAdapt=glo2usa |
| Momentary PushButton Switch - 12mm Square** | 2 | $0.00 | $0.00 | SparkFun | https://www.sparkfun.com/momentary-pushbutton-switch-12mm-square.html?srsltid=AU7gw4UYsga3kFomAPXouDmL9ocnQ9RkGAzC0S-DVtQuj2L2ftdCyW8-8WQ |
| **20 Pcs 10 Pairs 40 Pin 1x40 Single Row Male And Female 2.54 Breakable Pin Header PCB JST Connector Strip For Arduino DIY** | 1 | $0.00 | $0.00 | AliExpress | https://www.aliexpress.us/item/3256806803489511.html?src=google&src=google&albch=shopping&acnt=708-803-3821&isdl=y&slnk=&plac=&mtctp=&albbt=Google_7_shopping&aff_platform=google&aff_short_key=UneMJZVf&gclsrc=aw.ds&albagn=888888&ds_e_adid=&ds_e_matchtype=&ds_e_device=c&ds_e_network=x&ds_e_product_group_id=&ds_e_product_id=en3256806803489511&ds_e_product_merchant_id=5356860524&ds_e_product_country=US&ds_e_product_language=en&ds_e_product_channel=online&ds_e_product_store_id=&ds_url_v=2&albcp=19558607238&albag=&isSmbAutoCall=false&needSmbHouyi=false&gad_source=1&gad_campaignid=19566915268&gbraid=0AAAAAD6I-hFRHflJGCWNZNxA3pS6luCfe&gclid=CjwKCAjwotzWBhBFEiwA1JhPoMmyghtUCi_4KULXwjWdnLCmfAoaQBkmJ8YcMg8Dce4t1yKjeaI-DBoC0JwQAvD_BwE&gatewayAdapt=glo2usa |
| **ZeroneTeck USB C Data Cable** | 1 | $0.00 | $0.00 | Amazon | https://www.amazon.com/ZeroneTeck-Data-Cable-20Gbps-Video/dp/B0C9MGJM78/ref=sr_1_1?dib=eyJ2IjoiMSJ9.8Ki3FUlH49G5FGo5Ufavs8IjZDSj3mxA26y_Kr_BYi6OhzFPCxRu6dXn4Adf-hGm7GWa456uH7BhXOtopYR-iChs02o5soqe5FPaWtHmGnu0755S_S--Xs32kp9L1JWtnRe4WiggWJIQ24hPgj5bSWswg7Yb77u2gBnDziRMo7pHOsckFyGGR5RGgvoGr6aU6J0NPrKGbsFS5xVS748hzs4ZQwTm-sLvtqUqtIKdtcQ.0HA0KH58v7pFESOUe1QZHiOd3d2sX9bpWJfyq4IK85M&dib_tag=se&keywords=usb+c+data+cable&qid=1792555258&sr=8-1 |

* **Total Tax & Shipping for the whole order:** $17.69

---


   - *Make sure to change shipping to Global Standard Direct Line
   - *Make sure to change the Surface Finish from HASL (with lead) to LeadFree HASL

Things I already have/I'm buying myself:

1. Momentary PushButton Switch - 12mm Square x1
2. 20 Pcs 10 Pairs 40 Pin 1x40 Single Row Male And Female 2.54 Breakable Pin Header PCB JST Connector Strip For Arduino DIY x1
3. ZeroneTeck USB C Data Cable
   
  


