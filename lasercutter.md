#Laser Cutters

Laser cutters use computer numeric control (CNC) technology to accurately position a high-intensity laser over a sheet material. This allows precise engraving or cutting of the hseet material by light. Laser cutters are typically used for projects that require high precision but made of flat, 2D components. Unlike 3D printers, laser cutters cannot accomplish additive manufacturing, as they subtract material from a flat stock. 

Laser cutters are therefore highly recommended for parts that are flat-sheet based. 3D parts can also be designed to be made form individual flat components, which allows certain shapes to utilize the laser cutter as well. This is due to its efficiency. They are far more rapid than a 3D printer, as all material stock already exists (instead of having to melt them into place). This means the laser cutter is extremely useful in project cycles requiring rapid prototyping. Laser cutters can also be used for precision art and edge trimming, with a far smoother surface finish and an accuracy down to 1 thou on low-reflectivity materials (in the case of the P2S).

At Webb, there are two types of laser cutters. In the robotics room, there is an XTool P2S, which has a 55W CO2 based laser. In Studio A of the library innovation lab, there is a creality falcon pro, which is a 40W semiconductor diode laser. This tutorial will be going through the usage of these laser cutters and giving an example, a part from robotics, which can be efficiently manufactured via a laser cutter.

#Preparing for the Laser Cutter

First, the design of the target part is completed in a CAD software. As laser cutters work on 2D planar surfaces, they accept 2D design to calculate GCode positioning. For this section, we will be using the CAD program Onshape (found at https://onshape.com/), and use the DXF file format. Other file vector-based formats such as SVG files are accepted as well. However, they follow a similar process, but could involve additional software (eg. Adobe Illustrator).

A simple, 2D sketch can be exported using the "Export as DXF" button found when right-clicking a bounded area of the sketch.

For a part of a more complex object, such as a CAD model that involves thickness, right click the desired flat face on the 3D object. The face cannot be curved as laser cutters USUALLY work in a planar fashion. The XTool P2S is an exception to this rule; however, even with the 3D engraving feature, the machine does not process 3D files directly and must be converted into a greyscale image for contour mapping.


Example Project:
Pocketing a plate
