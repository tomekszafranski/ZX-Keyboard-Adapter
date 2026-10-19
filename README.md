# ZX-Keyboard-Adapter

## Do you need it?

When you build Sinclair ZX Spectrum clone or compatible machine you have to decide what kind of keyboard to use. If you are aiming for original case you will probably use original membranes with FFC tape connectors. If you are just experimenting or thinking about different case you can use one of more convenient modern versions. Most popular are probably [Superfo Harlequin 128 Keyboard](https://www.pcbway.com/project/shareproject/Supero_Harlequin_128_Keyboard.html) (with tactile switches) and [ZX Spectrum Keyboard](https://www.pcbway.com/project/shareproject/ZX_Spectrum_Keyboard.html) (with fully mechanical cherry-type switches). Those Harlequin keyboard are designed for Spectrum clone machines but they use wires or goldpin connectors that gives you more flexibility. If you are building your own version of the machine you are not even obliged to have two separate 8-pin and 5-pin connectors if only you can transfer all needed signals. Keyboard Adapter on one end connects to you machine with IDC16 connector and on the other end gives you the posibility to use both all original membranes and modern keyboards. It also works with ZX-81 allowing to use its keyboard for your Spectrum and mentioned above keyboards with ZX-81. 

## What is inside?

As for the connector, I have not found any standard so I followed reasonable pin assignment described in [ZX81 Keyboard Adventure](https://www.zx81keyboardadventure.com/p/zx-key-keyboard-guide-book.html). Inside IDC16 connector you have of course rows and columns of your keyboard.
In your Sinclair machine columns C0..C4 are connected to ULA pins KBD0..KBD4 and available on data bus D0..D4. Rows are not sequential - R0..R7 are connected to address bus A11, A10, A9, A12, A13, A8, A14, A15.  
For ZX-81, R2 and R3 are swapped so you need a configuration jumpers. Connect them horizontally if you want described above configuration (for ZX Spectrum) or connect them vertically if you want the swap (using ZX Spectrum keyboard with ZX-81 or ZX-81 keyboard with ZX Spectrum).

IDC16 connector can be stright or angled depending on yor needs. Of course, install only those connectors that you need.

<img width="1873" height="446" alt="37543cb3-16a9-45a7-988f-d1a97765d431" src="https://github.com/user-attachments/assets/91bd1160-9496-46b1-b79d-63b42f2b45e9" />

Have fun!

Tomek

> [!NOTE]
> **Disclaimer**: This is my project that I’ve built and it works for me. You can do it as well but remember, you’re responsible for your own doings and the consequences, not me.
>
> **Licensed under**: CERN Open Hardware Licence Version 2 - Strongly Reciprocal. Read [CERN-OHL-S](https://ohwr.org/cern_ohl_s_v2.txt)
