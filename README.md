# ZX-Keyboard-Adapter

## Do you need it?

When you build Sinclair ZX Spectrum clone or compatible machine you have to decide what kind of keyboard to use. If you are aiming for original case, you will probably use original membranes with FFC tape connectors. If you are just experimenting or thinking about your own case, you can use one of more convenient modern versions. Most popular are probably [Harlequin 128 Keyboard](https://www.pcbway.com/project/shareproject/Supero_Harlequin_128_Keyboard.html) (with tactile switches) and [ZX Spectrum Keyboard](https://www.pcbway.com/project/shareproject/ZX_Spectrum_Keyboard.html) (with fully mechanical cherry-type switches) - both by Superfo. Those Harlequin keyboard are designed for Spectrum clone machines but they use wires or goldpin connectors that gives you more flexibility. If you are building your own version of the machine you are not even obliged to have two separate 8-pin and 5-pin connectors, if only you transfer all needed signals. **Keyboard Adapter** on one end connects to you machine with IDC16 connector and on the other end, gives you the option to use both original membranes or modern keyboards. It also works with ZX-81, allowing to use ZX Spectrum keyboard with ZX-81 and vice versa. 

## What is inside?

As for the connector, I have not found any standard so I followed reasonable pin assignment described in [ZX81 Keyboard Adventure](https://www.zx81keyboardadventure.com/p/zx-key-keyboard-guide-book.html). Inside proposed IDC16 connector you have of course rows and columns from original design.
In your Sinclair machine columns C0...C4 are connected to ULA pins KBD0...KBD4 and available on data bus D0...D4. Rows are not sequential - R0...R7 are connected to address bus: A11, A10, A9, A12, A13, A8, A14, A15 in that order. Below you can see the setup (taken from original ZX Spectrum Service manual, edited by great Brendan Alford). Please notice that definition of columns and rows for this particular picture is different then generally accepted convention.

<img width="1539" height="866" alt="Zrzut ekranu 2026-10-19 125500" src="https://github.com/user-attachments/assets/870a7d8f-dbe6-4c0b-9947-fe0fce79f89f" />

For ZX-81, rows R2 and R3 are swapped so you need a configuration jumpers. Connect them horizontally if you want standard configuration for ZX Spectrum or connect them vertically if you want the swap - using ZX Spectrum keyboard with ZX-81 or ZX-81 keyboard with ZX Spectrum. As described in [ZX81 Keyboard Adventure](https://www.zx81keyboardadventure.com/p/zx-key-keyboard-guide-book.html) three remaining pins in IDC16 connector are used for +5V, GND, RESET in case there is more components on your keyboard side that need to be powered.

<img width="1398" height="341" alt="ZX-Keyboard-Adapter_board" src="https://github.com/user-attachments/assets/34566410-2399-4f27-bf8c-122bff936e26" />

<img width="1873" height="446" alt="37543cb3-16a9-45a7-988f-d1a97765d431" src="https://github.com/user-attachments/assets/91bd1160-9496-46b1-b79d-63b42f2b45e9" />

<img width="1760" height="1138" alt="efaf8720-1810-49bb-9128-c7fe4a2ea946" src="https://github.com/user-attachments/assets/f5aa1be8-85cb-4eca-b6e8-32b5badb0505" />

IDC16 connector used can be straight or angled depending on your needs. Of course, feel free to install only those connectors that you need.

Have fun!

Tomek

> [!NOTE]
> **Disclaimer**: This is my project that I’ve built and it works for me. You can do it as well but remember, you’re responsible for your own doings and the consequences, not me.
>
> **Licensed under**: CERN Open Hardware Licence Version 2 - Strongly Reciprocal. Read [CERN-OHL-S](https://ohwr.org/cern_ohl_s_v2.txt)
