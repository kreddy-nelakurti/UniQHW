# UniQHW

The hardware repository for UQ Phone (UniQ)
The Corresponding software component can be found [https://github.com/Benksur/UniQOS](https://github.com/Benksur/UniQOS)

## About

**Supervised by:** Professor Pauline Pounds  
**Institution:** University of Queensland
<div align="center">

### UQ Phone Team (Year 1 - 2025)

| Name | Role |
|------|------|
| **Ty Behnke** | Firmware Design |
| **James Wood** | Hardware Design |
| **Caiyan Jin** | UI/UX Design |
</div>

Any Questions about the PCB and Schematics please direct them to [james.brian.wood@outlook.com](james.brian.wood@outlook.com)

## Production

The V0.2.0 PCB's must be made with the following specifications from JLCPCB

### Main PCB

This 6-Layer PCB must be made with the following

- Via Covering:	Epoxy Filled & Capped
- Min via hole size/diameter:	0.2mm/(0.3/0.35mm)

The following are also required if meeting the full size specifications of UniQ

- PCB Thickness:	0.8mm

Production versions should also be made with the following (Dependant on desired finish)

- Surface Finish:	ENIG Gold Thickness: 2U"
- PCB Color:	Black
- Silkscreen:	White

### Secondary PCB (Cellular Board)

This 4-Layer PCB must be made with the following

- PCB Thickness:	0.6mm
- Via Covering:	Epoxy Filled & Capped
- Min via hole size/diameter:	0.2mm/(0.3/0.35mm)
- Specify Stackup:	yes JLC04061H-2116

If Either the thickness or stackup is to change this boards traces should be redesigned for 50Ohm Impedance 

Production versions should also be made with the following (Dependant on desired finish)

- Surface Finish:	ENIG Gold Thickness: 2U"
- PCB Color:	Black
- Silkscreen:	White


## Current Issues And Improvements

The V0.2.0 PCB currently suffers from several issues which should be rectified on later versions:

- Batter Connector Location: move so it can be inserted and removed indpendantly of the secondary PCB
- SD/SIM Socket: Tie 3.3v SD card rail to insertion detection to prevent hot-plugging
- Debug Pads: Consider moving to provide easier access without interferance from screen
- Soft Power: Add soft power switch for more agressive power-off functionality and safer power-downs

The following may also be investigated for benefit 
- Improve Display: Ideally Display utilises a parellel interface, this needs more investigation
- Audio Volume: Current speaker is quiet, this should be investigated further to see if this can be remediated in firmware first
- USB Support: Add USB data connectivity to the device for file transfer or programming, this may resolve debug pad issues
- BT Audio: this poses significant challenges, although may be worth while, investigate further

