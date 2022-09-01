# Static and Dynamic Marker Position Verification - CMAS standards QA Test in Visual3D 
	
### Overview	
This pipeline script (.v3s) and Visual 3D report template (.rgt) is what we use in the Derby lab as a 3D motion system  test  to meet item 2.8 of the CMAS standards (v15, 2021). It tests:
**_"
	a) The absolute position of static markers in capture volume;  b) The relative marker position in capture volume during a dynamic test e.g. the distance between fixed markers through the whole volume 
"_**

### Experimental Setup
4 markers are placed on the floor at each corner of the forceplate area. We have 4 plates (60 x 40cm) in a linear configuration
In Derby we have a CalTester rod but any pole with markers fixed at a known distance apart would be sufficient, adapting code to suit marker names
A short acquisition is taken (~40s) in which the rod is moved and rotated through the capture volume before being rested on its baseplate

### Processing Instructions
1. If using a CalTester, label its markers and the floor markers in whichever tracking software you have, using the labelling arrangement shown below and then save the file as a .c3d
2. Load the .c3d file to the visual 3d workspace  (Example data file in the repository)
3. Load and run the pipeline script
4. Open the report template (although the pipeline script will open this anyway, if the filepath is specified) and enter the date of the acquisition by editing the page title.
The report template displays graphs of the absolute positions of the 4 floor markers alongside a table of their average reconstructed coordinates. Also, graphs of the rod marker positions provide a means of assessing how well the CalTester rod has been moved throughout the capture volume during the acquisition. 
The distances between markers in the 2 planes on the floor are communicated through graphs of ‘Forceplate area width and length’ as well as the distance between top and bottom markers of the caltester rod.
### Requirements
Visual 3d ([C-motion](https://www.c-motion.com/)). Any version should work but we are currently running version 6.

### Other Notes

These instructions assume you already have a working knowledge of Visual 3D and will be able to modify the pipeline code and report template to suit your lab's force plate setup, but I'm happy to try and help out if you're experiencing problems doing so.

### Contact 
martin.kerr1@nhs.net

![image](https://user-images.githubusercontent.com/50867224/187958788-edf6034e-6c6e-437f-beaf-c805a83e96bd.png)

![image](https://user-images.githubusercontent.com/50867224/187958531-f9a97f74-d5eb-46df-ba4e-6eabb032799a.png)

