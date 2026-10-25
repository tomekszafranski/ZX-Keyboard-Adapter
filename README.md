# ZX-Keyboard-Adapter

## Do you need it?

When you build Sinclair ZX Spectrum clone or compatible machine, you have to decide what kind of keyboard to use. If you are planning to utilize original case, you will probably use original membranes with FFC tape connectors. If you are just experimenting or thinking about your own case, you can use one of more convenient modern keyboard versions. Probably the most popular are [Harlequin 128 Keyboard](https://www.pcbway.com/project/shareproject/Supero_Harlequin_128_Keyboard.html) (with tactile switches) and [ZX Spectrum Keyboard](https://www.pcbway.com/project/shareproject/ZX_Spectrum_Keyboard.html) (with fully mechanical cherry-type switches) - both by Superfo. Those Harlequin keyboards are designed for Spectrum clone machines but use wires or goldpin connectors that gives you more flexibility while connecting. If you are building your own version of the machine you are not even obliged to have two separate 8-pin and 5-pin connectors, if only you transfer all needed signals. Proposed **Keyboard Adapter** on one end connects to your machine with IDC16 connector and on the other end, gives you the option to use original membranes or modern keyboards. It also works with ZX-81, allowing to use ZX Spectrum keyboard with ZX-81 and vice versa. 

## What is inside?

As for the connector, I have not found any standard so I followed reasonable pin assignment described in [ZX81 Keyboard Adventure](https://www.zx81keyboardadventure.com/p/zx-key-keyboard-guide-book.html). Inside proposed IDC16 connector you have of course rows and columns from original design.
In your Sinclair machine columns C0...C4 are connected to ULA pins KB0...KB4 and available on data bus D0...D4. Rows are not sequential - R0...R7 are connected to address bus: A11, A10, A9, A12, A13, A8, A14, A15 respectively. The setup is described in section 1.8 of [ZX Spectrum Service Manual](https://spectrumforeveryone.com/wp-content/uploads/2017/08/ZX-Spectrum-Service-Manual.pdf) by Sinclair. Please note that definition of columns and rows there is opposite to generally used convention.

For ZX-81, rows R2 and R3 are swapped so you need a configuration jumpers (see below). Connect them horizontally if you want standard configuration for ZX Spectrum or connect them vertically if you want the swap - using ZX Spectrum keyboard with ZX-81 or ZX-81 keyboard with ZX Spectrum. As described in [ZX81 Keyboard Adventure](https://www.zx81keyboardadventure.com/p/zx-key-keyboard-guide-book.html) three remaining pins in IDC16 connector are used for +5V, GND and RESET - in case there are components on your keyboard side that need to be powered.

<img width="1361" height="320" alt="ZX-Keyboard-Adapter_board" src="https://github.com/user-attachments/assets/693347f6-4f33-4a3b-b5b4-4e4a7d8d97d3" />

<img width="1760" height="1138" alt="efaf8720-1810-49bb-9128-c7fe4a2ea946" src="https://github.com/user-attachments/assets/f5aa1be8-85cb-4eca-b6e8-32b5badb0505" />

IDC16 connector can be straight or angled depending on your needs. Of course, feel free to install only those connectors that you need.

Have fun!

Tomek

> [!NOTE]
> **Disclaimer**: This is my project that I’ve built and it works for me. You can do it as well but remember, you’re responsible for your own doings and the consequences, not me.
>
> **Licensed under**: CERN Open Hardware Licence Version 2 - Strongly Reciprocal. Read [CERN-OHL-S](https://ohwr.org/cern_ohl_s_v2.txt)
