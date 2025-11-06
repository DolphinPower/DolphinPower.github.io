# Laser Cutters

Laser cutters use computer numeric control (CNC) technology to accurately position a high-intensity laser over a sheet material. This allows precise engraving or cutting of the hseet material by light. Laser cutters are typically used for projects that require high precision but made of flat, 2D components. Unlike 3D printers, laser cutters cannot accomplish additive manufacturing, as they subtract material from a flat stock. 

Laser cutters are therefore highly recommended for parts that are flat-sheet based. 3D parts can also be designed to be made form individual flat components, which allows certain shapes to utilize the laser cutter as well. This is due to its efficiency. They are far more rapid than a 3D printer, as all material stock already exists (instead of having to melt them into place). This means the laser cutter is extremely useful in project cycles requiring rapid prototyping. Laser cutters can also be used for precision art and edge trimming, with a far smoother surface finish and an accuracy down to 1 thou on low-reflectivity materials (in the case of the P2S).

At Webb, there are two types of laser cutters. In the robotics room, there is an XTool P2S, which has a 55W CO2 based laser. In Studio A of the library innovation lab, there is a Creality Falcon 2 Pro, which is a 40W semiconductor diode laser. This tutorial will be going through the usage of these laser cutters and giving an example, a part from robotics, which can be efficiently manufactured via a laser cutter.

## Preparing for the Laser Cutter
First, the design of the desired part is completed in a CAD software. 

As laser cutters work on 2D planar surfaces, they accept 2D design to calculate GCode positioning. For this section, we will be using the CAD program Onshape (found at https://onshape.com/), and use the DXF file format. Other file vector-based formats such as SVG files are accepted as well. However, they follow a similar process, but could involve additional software (eg. Adobe Illustrator).

A simple, 2D sketch can be exported using the "Export as DXF" button found when right-clicking a bounded area of the sketch. This exports the continugous face, that the mouse is currently part of.

For a part of a more complex object, such as a CAD model that involves thickness, right click the desired flat face on the 3D object. The face cannot be curved as laser cutters USUALLY work in a planar fashion. The XTool P2S is an exception to this rule; however, even with the 3D engraving feature, the machine does not process 3D files directly and must be converted into a greyscale image for contour mapping.

**IMPORTANT:** whenever using the XTool P2S or the Creality Falcon 2 Pro, the DXF **MUST** be exported in units of **MILLIMETERS**. This is the default working unit for both lightburn and XTool Creative Space, the software used to process the DXF file into instructions to the laser cutter. Unless you have manually changed the unit in the software to something else, assume default settings and use millimeters. The unit can be selected in a pop up menu in Onshape when confirming the DXF file export.

## Using the XTool P2S
Observe the XTool P2S. The laser cutter is comprised of a flat, rectangular cutter body, a filter module on the side and a long and thin vent wall panel used to block out the fumes, connected to the filter and laser cutter via an air pipe. 
The first step is to turn on the filter module, with the switch located on the front side, then turn the dial on the right side of the module to maximum. Open the window of the robotics lab, then go outside. From the outside, pass the entire white wall vent panel through the window. From the outside, the black sliding window frame has two distinct slots, with notches separating them. Identify the second slot, which is the one furthest towards the indoors. Raise the wall panel and slide the top of the panel into the second slot, making sure the vent side faces out and the duct side faces in. Slide the bottom of the panel into the same slot, then close the window. The window should securely squeeze the wall panel into the wall, with the sponse seal contacting the window frame the entire way up. The setup is now complete.

Identify the power switch on the back right corner of the laser cutter and turn the laser cutter on. The screen and round button on the top of the laser cutter should light up. Observe that the laser cutter auto homes its cutting head. Go back to the computer and start up a new project in XTool Creative Space, the software used to send designs to the XTool P2S. Open up a new project. This should lead to an interface with a white grid in the middle, a toolbar on the left and on top, and some options on the right. 

Connect the computer to the wifi "Webb", as this will allow wireless connectivity to the laser cutter. Locate the connection button on the top right, shaped like two arrows facing opposite directions. Clicking the connect button should show a menu. If the laser cutter is already shown, press the Connect button on the right. If it is not shown, click the connect device text in the bottom, select Wi-Fi mode and then find the laser cutter in the list of wifi devices. Alternatively, use a USB-C data cable, plugging one end into the computer and another end into the corresponding port on the left side of the laser cutter.

Once the laser cutter is connected, an image of the laser cutter's camera should automatically appear on the screen. The option to refresh the image is located on the icon shaped like a camera with a refresh symbol inside.

Place a piece of stock material in the laser cutter, whether that be acrylic, wood (MDF / eucaboard), cardboard, corrugated plastic or others. Note that cutting polycarbonate is currently not supported by the filters. Remember the type of material and thickness of material. Refresh the camera in the XTool Creative Space. Go to the top right of the screen, and click on the text "Unknown material". Select the desired material and thickness from the menu. 

Then, drag the DXF file into the center grid area, where the camera image overlay now is. A black outline of the DXF should appear. Place this over the desired (uncut) region of the stock material according to the imagery from the camera. The DXF file may also be adjusted by groups. By right-clicking, text with the same properties can be grouped together, which helps make selecting modes for each step more efficient.

After placing the DXF in its desired spot and using the measurement tool (found in the left menubar) to verify its dimensions, use the mode selector in the panel on the right to select either score, engrave or cut, depending on the nature of the project. Different groups of geometries can be assigned to different operations. After each operation is selected, set a laser power and head movement speed. The higher the power, the more intense the cut, but could result in elevated fire risks. The faster the speed, the more faster the cut completes, but too much speed could result in the laser not having enough time to burn through material. The XTool provides a grid which visualizes what each material results in for a certain range of presents of powers and speeds. A setting can be selected in the preset diagram by clicking one of the result options; a custom setting can be set using the sliders as well.

## Using the Falcon 2 Pro

Example Project:
Pocketing a plate
