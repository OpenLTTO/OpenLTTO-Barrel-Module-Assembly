# OpenLTTO
The OpenLTTO Project is an attempt to recreate the Lazer Tag Team Ops protocol, and game system, in a completely open-source solution. Eventually our intent, is to expand on the LTTO system, adding new functionality, and features, while maintaining backwards compatibility with this classic Lazer Tag gear.

> This Project wouldn't be possible without all the hard work of Richie Mickan https://github.com/rmick
> His work on recreating the LTTO Protocol, and the development of the Combobulator app are core to the firmware and capabilities of this project.

> Additionally this is built on top of the excellent product developed and released by Hasbro/Tiger Electronics. And the work done by Tag Ferret to release the technical specs, and unlock much of the magic of the protocol, and the inner workings.

We intend to do this via a collection of open-source hardware components that can act as building blocks, to build anything you might require for a Lazer Tag game (Taggers, Hosting Pods, Zone controllers, utilities, etc). And an opensource firmware to operate it all. 

Shield: [![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg

# OpenLTTO Barrel Module Assembly
The OpenLTTO Barrel Module Assembly is a 3D Printable Optical Assembly, which houses the Barrel Module PCB, and required optics, inside a simple assembly which can then be easily embedded within other projects.

The primary place this design is authored is on OnShape CAD as a publicly shared document, accessible at the following link:
https://cad.onshape.com/documents/e1d899f96e1e04d7275a09a1/w/607acbe0bebce4cc9caf4ee5/e/436bfff928f4fe3aca254f6f?configuration=default&renderMode=0&uiState=65be94fa0f24c16241198061

Included in this repo are the following resources:
- This Readme File, for informational purposes
- STL files of "Side A" and "Side B" of the main optical tube assembly
- STL files of "Focusing Spacers" which can be inserted alongside the lens to shift the position for focus
- A STEP file of the entire project

Currently these exports are only done with a single setup, for a 25mm diameter, 3mm thickness, focusing lens, with a focal distance of 76.2mm (commonly available ZnSe lenses for focusing IR laser cutters). This lens configuration optimally makes use of available space for the LED output, however, there are less expensive lenses available, and the assembly can be tuned through simple configuration parameters to accommodate other lense sizes. Eventually once we have confirmed performance of these options, we will release specific exports for particular lens models, along with a link for where to acquire the lens.

The PCB is currently designed to accommodate lenses up to 27mm in diameter, but no larger. The assembly will accept lenses in it's parametric input of 16mm through 27mm diameter.

# Using the assembly in a project

The assembly is designed to be mechanically retained via it's shape, and a keyed slot running it's length. The slot is designed to be retained at the rear only, allowing the assembly to be an "unknown length". This is to accommodate multiple focal length configurations in the future. Changing the lens configuration within the accepted bounds will not alter the outside shape of the assembly, other than it's overall length (related primarily to focal length).

This should allow the design of taggers for example, which can universally accommodate any focal length module, within design constraints (ie: a pistol, may accept anything below an overall module length of 105mm which correlates approximately to a 76.2mm focal length. While a rifle may accept anything below a 180mm total length, which correlates approximately to a focal length of 150mm. Longer focal lengths are possible as well, though are likely to be sub optimal without first finding an alternative emitter LED for the PCB which has a much tighter angle of half intensity.

If not using CAD to design the tagger, or other housing, the dimensions of the assembly are as follows:
- Approximately oval shape in the width/height plane
- Overall Width 58.5mm
- Overall Height 
- End Radius 15.2mm
- Minimum total length approximately 30mm longer than the focal length, for a focal length of 40mm (the shortest commonly available for 25mm lens) the resulting total length would be 70mm long
- The keyway front face is 9.1mm from the rear face
- The keyway is approximately 3.3mm deep, and 8.65mm wide at the bottom, with sides that angle out at 45 degrees.
- The rear of the assembly requires clearance for the electronics of approximately 5mm


