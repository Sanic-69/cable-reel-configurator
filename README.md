DISCLAIMER: AI WAS USED FOR THIS!
---------------------------------

As I know that there will be at least one Person who will be mad about this, I thought I would be open about this from the start.
YES, I used ChatGPT to correct and repackage my code (God knows i cant make it as efficient as those AIs can) BUT NO, this Project is NOT entirely AI Generated.
The Idea, aswell as the PoC was done by me, but I felt the need to "clean up" everything for the GitHub release, so here we are.


Modular Cable Spool Web Configurator
===================================

A parametric, workshop-grade cable spool system with a web-based configurator
and OpenSCAD-based STL generation.

This project allows users to calculate and generate 3D-printable cable spools
based on real cable parameters such as diameter, length, and mounting method.

Designed for PETG, workshop environments, and 256×256×256 mm print volumes.


My Goals for this Project:
-------------------------

- Generate correctly sized cable spools from real-world cable data
- Provide a simple web-based configurator
- Export OpenSCAD configuration files (config.scad)
- Enable reproducible and version-controlled STL generation
- Support modular workshop systems (rack or standalone)


Features I (probably) didn't screw up (...yet):
----------------------------------------------

- Web-based configurator (HTML + JavaScript)
- Parametric calculation of spool dimensions
- Automatic print-bed size validation
- OpenSCAD-based geometry (single source of truth)
- config.scad export via browser download
- Optimized for PETG and workshop use
- Modular system (spool, rack mount, stand foot)


Recommended Use:
---------------

1. Open the web configurator (index.html)
2. Enter cable parameters:
   - Cable diameter
   - Cable length
   - Spool width
   - Axis diameter
   - Mounting mode
3. Click "Export config.scad"
4. Copy the generated config.scad into the OpenSCAD folder
5. Open OpenSCAD and render the model
6. Export STL files for 3D printing


The Project Structure:
---------------------

cable-reel-configurator/

│

├─ web/

│  └─ index.html        Web configurator UI

│

├─ openscad/

│  ├─ spool.scad        Parametric cable spool

│  ├─ foot.scad         Standalone foot module

│  ├─ rod_mount.scad    Rack / rod mounting module

│  └─ config.scad       Auto-generated configuration

│

├─ export/              Generated STL files (not tracked)

│

├─ LICENSE

└─ README.txt


My Printing Recommendations:
---------------------------

- Material: PETG
- Nozzle: 0.6 mm
- Layer height: 0.28 mm
- Infill: 15–20 % (Gyroid)
- Perimeters: 4 or more
- Orientation: Print spool lying flat


What I still want to do:
-----------------------

- Automatic module selection in OpenSCAD
- STL export presets
- Rack system designer
- Cable type presets (power, LAN, air hose)
- Versioned releases


My Motivations:
--------------

White Monster
Cigarettes (don't smoke Kids, its bad for you!)

Contributions and pull requests are welcome.
