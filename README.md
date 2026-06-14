# DIY_Mini_Marauder

This is an open source version of --------------------
## The Poster
*still in the making*

## The Design
### The PCB
![PCB](./Media/KiCad/marauder%20PCB.png)
### The Schematics
![Schematics](./Media/KiCad/marauder%20Schematic.png)
### The Enclosure Case 
With the device inside:
![Device](./Media/Fusion360/Device.png)

Empty:
![Assmebled](./Media/Fusion360/Assembled.png)


## Assembly
### Step Files
All of the step files can be downloaded [here](./Step_Files/).

### Assembly video
(to be uploaded using github's MD editor)

## Firmware
### Fzee flasher (Marauder Mini)
- Visit the [FZEE FLASHER](https://fzeeflasher.com/) website
- Make sure your device is connected to your PC
- Click "Connect" <br>
<img width="181" height="48" alt="image" src="https://github.com/user-attachments/assets/b4bb688b-bfb8-464b-a4da-e55b52c00563" />

- Select the Programmer chip for your device (which would be CP2104 if you used the schematics/PCB in this repository) <br>
<img width="429" height="423" alt="image" src="https://github.com/user-attachments/assets/c400aff8-7c54-443b-a0f2-ba439f48c2e2" />

- If you used the schematics/PCB provided in this repository, then you can skip this step. <br>
As soon as you see this screen, hold down the BOOT button on your device as the flasher will automatically reset the device and it will go into the boatloader mode <br>
<img width="273" height="76" alt="image" src="https://github.com/user-attachments/assets/71b266a3-5740-4abd-a3f9-4292a7f7828a" />

- Select "ESP32 Marauder Mini Device" <br>
<img width="628" height="439" alt="image" src="https://github.com/user-attachments/assets/168cee87-4439-4ad7-864f-fa4af325aa8e" />

- Select the latest version <br>
<img width="170" height="129" alt="image" src="https://github.com/user-attachments/assets/3831aca0-2004-409e-9db8-04e21e200db1" />

- Select "Marauder" as the firmware <br>
<img width="181" height="128" alt="image" src="https://github.com/user-attachments/assets/129829b3-ea91-42cd-a314-d73268ddc1c5" />

- Erase the device first to make sure that it's not affected by any previously installed firmwares <br>
<img width="1129" height="547" alt="image" src="https://github.com/user-attachments/assets/3557a42a-3f0c-4f88-8353-aef243760d9d" />

- Click "Program" <br>
<img width="1113" height="575" alt="image" src="https://github.com/user-attachments/assets/825e864c-5778-4fc1-a418-72125d1ae0d5" />

- It will take arround 10 seconds to flash the firmware.  <br>
  After those 10 seconds, you should see this screen which indicates that you succesfully flashed the device with the new firmware: <br>
  <img width="505" height="61" alt="image" src="https://github.com/user-attachments/assets/414fb868-b80e-4891-9937-c8a1bc804162" />



### Bruce (Bruce's Firmware)
- Visit [Bruce's Web Firmware Flasher](https://bruce.computer/flasher) 
- Select whatever release you want (it's recommended to select the latest release)
 <img width="570" height="142" alt="image" src="https://github.com/user-attachments/assets/7f779d35-56f8-49f3-9cdc-c99741975e87" />
 
- Select "Custom Boards"
<img width="1438" height="115" alt="image" src="https://github.com/user-attachments/assets/46af4877-1ab4-47ea-ac86-ba6ab39f025c" />

- Select "Marauder Mini"
<img width="1688" height="232" alt="image" src="https://github.com/user-attachments/assets/e01ff70b-297f-4254-a239-439757cc3c3c" />

- Select "Connect to Device"
<img width="390" height="178" alt="image" src="https://github.com/user-attachments/assets/3d82d22e-7f21-4564-bf3d-79527dd0dcb0" />

- Select the Programmer chip for your device (which would be CP2104 if you used the schematics/PCB in this repository)
<img width="421" height="413" alt="image" src="https://github.com/user-attachments/assets/23b841e9-3e63-418b-ba16-42bf6b7ddac1" />

- Select "Instal Marauder-Mini"
<img width="305" height="244" alt="image" src="https://github.com/user-attachments/assets/90c4378e-641e-4aeb-b3c3-85e0433d8db5" />

- Then make sure to have the "Erase device" option enabled then click next
<img width="586" height="285" alt="image" src="https://github.com/user-attachments/assets/9c754400-10ed-4c5b-a5fa-2a80364ab52e" />

- Confirm the instalation
<img width="315" height="264" alt="image" src="https://github.com/user-attachments/assets/3e93bfa5-14b2-4c7b-a6cf-b434a5369e3e" />

- If you used the schematics/PCB provided in this repository, then you can skip this step. <br>
As soon as you see this screen, make sure to put your device into the bootloader mode by holding the BOOT button down, pressing the RST button, and then after 2 seconds release the BOOT button.
<img width="309" height="213" alt="image" src="https://github.com/user-attachments/assets/41a3e569-285f-4a53-a02d-a6363ff1248c" />

- It will take around 2 minutes to upload the firmware. <br>
After those 2 minutes, you should see this screen which indicates that you had a succesful instalation:
<img width="300" height="239" alt="image" src="https://github.com/user-attachments/assets/fd29074a-138c-4ad8-b7fc-c1319ceb3247" />



## Buttons and leds
### The two LEDs
Next to the USB-C port there are 2 LEDs: <br>
- The white one indicates wether the device is powered or not. <br>
- The blue one indicates wether the device is recieved power from the USB-C port or not (which is used to charge the battery).

### The two buttons on the back of the device and their functions
- The Upper button is used to put the ESP32 into the bootloader mode (AKA. the BOOT button). <br>
- The lower button is used to reset the device (AKA. the RST button).<br>

### The side switch
- The side switch is used to power the device ON or OFF.

## BOM
### BOM table (components only)
|Name                            |Value                       |Link                                                                                                                                                                                                                                                                                                                                                                    |Cost (EGP) per one|Cost (USD)|Total Cost (EGP)                           |Total Cost (USD)|Qty of packages|Description          |quantiy per pack|
|--------------------------------|----------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------|----------|-------------------------------------------|----------------|---------------|---------------------|----------------|
|Capacitor                       |100nF                       |https://lampatronics.com/product/smd-multilayer-ceramic-capacitor-0805-2012-104-100nf-50v-1pcs-2                                                                                                                                                                                                                                                                        | EGP 1.00         | $0.02    | EGP 3.00                                  | $0.06          |3              |                     |1               |
|Capacitor                       |4.7uF                       |https://lampatronics.com/product/smd-multilayer-ceramic-capacitor-1206-4-7uf-16v-1pcs                                                                                                                                                                                                                                                                                   | EGP 1.50         | $0.03    | EGP 4.50                                  | $0.09          |3              |                     |1               |
|Capacitor                       |2.2uF                       |https://lampatronics.com/product/smd-multilayer-ceramic-capacitor-0805-2-2uf-50v-1pcs                                                                                                                                                                                                                                                                                   | EGP 1.00         | $0.02    | EGP 1.00                                  | $0.02          |1              |                     |1               |
|SD Card slot                    |TF-115                      |https://lampatronics.com/product/push-push-type-tf-micro-sd-card-socket-adapter-automatic-pcb-connector                                                                                                                                                                                                                                                                 | EGP 8.00         | $0.15    | EGP 8.00                                  | $0.15          |1              |                     |1               |
|Charging LED                    |SZYY0603Y                   |https://lampatronics.com/product/smd-led-0805-blue-10pcs                                                                                                                                                                                                                                                                                                                | EGP 8.00         | $0.15    | EGP 8.00                                  | $0.15          |1              |Charge LED (RED)     |10              |
|Power LED                       |SZYY0603Y                   |https://lampatronics.com/product/smd-led-0805-white-10pcs                                                                                                                                                                                                                                                                                                               | EGP 8.00         | $0.15    | EGP 8.00                                  | $0.15          |1              |Power LED (White)    |10              |
|Schottky Diode                  |MBR120LSF (alt: 1N5819 SS14)|https://uge-one.com/product/smd-schottky-diode-1n5819-ss14-1a-40v-sma-package/                                                                                                                                                                                                                                                                                          | EGP 2.50         | $0.05    | EGP 2.50                                  | $0.05          |1              |Schottky             |1               |
|JST Connector                   |S2B-PH-SM4-TB               |https://uge-one.com/product/jst-connector-male-polarized-xh2-54-2p/                                                                                                                                                                                                                                                                                                     | EGP 1.14         | $0.02    | EGP 1.14                                  | $0.02          |1              |JST connector        |1               |
|BOOT and RESET transistors      |S8050                       |https://lampatronics.com/product/s8050-transistor-40v-0-5a-npn                                                                                                                                                                                                                                                                                                          | EGP 0.50         | $0.01    | EGP 1.00                                  | $0.02          |2              |RST&BOOT transistors |1               |
|Power management and TFT LED PWM|AO3401                      |https://uge-one.com/product/ao3401-sot23-general-purpose-p-channel-mosfet-smd-transistor-sot-23/                                                                                                                                                                                                                                                                        | EGP 3.00         | $0.06    | EGP 6.00                                  | $0.12          |2              |Power manage, TFT LED|1               |
|Resistor                        |5.1k                        |https://uge-one.com/product/smd-chip-resistor-size-0603-5-1k-ohm/                                                                                                                                                                                                                                                                                                       | EGP 0.50         | $0.01    | EGP 1.00                                  | $0.02          |2              |USB-C resistors 5.1k |1               |
|Resistor                        |10K                         |https://lampatronics.com/product/smd-resistor-10kohm-103-0805-10pcs                                                                                                                                                                                                                                                                                                     | EGP 2.00         | $0.04    | EGP 4.00                                  | $0.08          |2              |                     |10              |
|Resistor                        |1K                          |https://lampatronics.com/product/smd-resistor-1kohm-102-0805-10pcs                                                                                                                                                                                                                                                                                                      | EGP 2.00         | $0.04    | EGP 2.00                                  | $0.04          |1              |                     |10              |
|Prog Resistor                   |2K                          |https://lampatronics.com/product/smd-resistor-2kohm-202-0805-10pcs                                                                                                                                                                                                                                                                                                      | EGP 2.00         | $0.04    | EGP 2.00                                  | $0.04          |1              |                     |10              |
|RST and BOOT buttons            |SW_Omron_B3FS               |https://lampatronics.com/product/smd-push-button-3425mm-tactile-tact-micro-switch-momentary-4pin                                                                                                                                                                                                                                                                        | EGP 3.00         | $0.06    | EGP 6.00                                  | $0.12          |2              |                     |1               |
|LDO Enable Switch               |K3-1296S-E1_C128955         |https://uge-one.com/product/horizontal-small-slide-toggle-switch-spdt-3pin-2mm-pin-spacing-sk12d02vg7/                                                                                                                                                                                                                                                                  | EGP 4.00         | $0.08    | EGP 4.00                                  | $0.08          |1              |Power slide switch   |1               |
|directional buttons             |                            |https://lampatronics.com/product/push-button-4pin-long-6x6x13mm                                                                                                                                                                                                                                                                                                         | EGP 1.50         | $0.03    | EGP 7.50                                  | $0.14          |5              |Directional switch   |1               |
|MCU                             |ESP32-WROOM-32              |https://uge-one.com/product/espressif-esp32-wroom-32-dual-core-wi-fi-bluetooth-iot-module/                                                                                                                                                                                                                                                                              | EGP 290.00       | $5.58    | EGP 290.00                                | $5.58          |1              |MCU                  |1               |
|Battery charger                 |MCP73831T-2ACI_OT           |[Long Aliexpress link](https://ar.aliexpress.com/item/32844180448.html?spm=a2g0o.productlist.main.1.3ce63cd6piQzMy&algo_pvid=c4aa9c81-0eb9-4713-ae7a-3ae3d38d7e01&pdp_ext_f=%7B%22order%22%3A%22167%22%2C%22spu_best_type%22%3A%22price%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A32844180448%7C_p_origin_prod%3A)| N/A              | $4.28    | N/A                                       | $4.28          |1              |Battery Charger      |10              |
|Programmer                      |CP2104                      |[Long Aliexpress link](https://ar.aliexpress.com/item/1005012309258723.html?pdp_ext_f=%7B%22sku_id%22%3A%2212000058021215527%22%7D&sourceType=1&spm=a2g0o.wish-manage-home.0.0&gatewayAdapt=glo2ara)                                                                                                                                                                    | N/A              | $1.97    | N/A                                       | $1.97          |1              |USB to TTL chip      |1               |
|LDO Regulator                   |MIC5219-3.3YM5              |[Long Aliexpress link](https://ar.aliexpress.com/item/1005006130724980.html?spm=a2g0o.productlist.main.6.4c73EOI6EOI6w7&algo_pvid=ba305fa5-d1fa-45ea-b339-9e0b52087c6d&pdp_ext_f=%7B%22order%22%3A%2222%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005006130724980%7C_p_origin_prod%3A)   | N/A              | $4.23    | N/A                                       | $4.23          |1              |LDO regulator        |10              |
|Display                         |TFT_1.44                    |[Long Aliexpress link](https://ar.aliexpress.com/item/1005001598020071.html?spm=a2g0o.order_list.order_list_main.5.714d1802IvCG36&gatewayAdapt=glo2ara)                                                                                                                                                                                                                 | N/A              | $2.16    | N/A                                       | $2.16          |1              |                     |1               |
|USB-C                           |USB_C_Receptacle_USB2.0_16P |https://www.ram-e-shop.com/shop/usb9-c-type-pcb-usb-connector-on-pcb-c-type-type-female-16-pin-sku-usb9-8125                                                                                                                                                                                                                                                            | EGP 5.00         | $0.10    | EGP 5.00                                  | $0.10          |1              |                     |1               |
|Battery                         |700 mah                     |https://lampatronics.com/product/battery-polymer-3-7v-700mah-li-ion-single-cell-35x20x5mm-502035                                                                                                                                                                                                                                                                        | EGP 135.00       | $2.60    | EGP 135.00                                | $2.60          |1              |                     |1               |
|M5 Screws                       |M5*16mm                     |https://store.fut-electronics.com/products/screw-m5x16mm-hexagonal-head?_pos=15&_sid=376b1bf88&_ss=r                                                                                                                                                                                                                                                                    | EGP 2.00         | $0.04    | EGP 2.00                                  | $0.04          |1              |                     |1               |
|                                |                            |                                                                                                                                                                                                                                                                                                                                                                        |                  |          |                                           |                |               |                     |                |
|                                |                            |                                                                                                                                                                                                                                                                                                                                                                        |                  |          | EGP 501.64                                | $22.29         |               |                     |                |
|                                |                            |                                                                                                                                                                                                                                                                                                                                                                        |                  |          | (Stuff from aliexpress not included here) |                |               |                     |                |

### Orders from different manufacturers
#### In Egypt
to be finished
#### Out of Egypt
JLCPCB (both PCB and case)
<img width="1434" height="724" alt="image" src="https://github.com/user-attachments/assets/cff0abbd-560b-4fbe-9da5-c764f21fd100" />

<br>
<br>
<br>
<br>
> The firmware is designed by [JustCallMeKoko](https://github.com/justcallmekoko). <br>
The PCB that was reverse engineered for the making of [DIY Mini Marauder](https://github.com/mkhairyx/DIY_Mini_Marauder) is designed by [JustCallMeKoko](https://github.com/justcallmekoko). <br>
This repo and all of it's contents were Designed by [@mkhairyx](https://github.com/mkhairyx).<br>
Supported by [Fallout](https://fallout.hackclub.com/) and [Hack Club](https://hackclub.com).<br>

