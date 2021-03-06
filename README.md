# hp-41_hours

**NOTE:** This program is part of the ISENE.ROM (https://github.com/isene/hp-41_isene-rom). The FOCAL listing can be found in the "src" folder of that project. Any updates and new version will be found there.

A customized program for tracking hours worked on projects.

There exists a simple hour registration program in the ISENE.ROM (https://github.com/isene/hp-41_isene-rom). This program expands the functionality to make it easier to enter hours when you are working for several (up to 5) different projects simultaneously. To use this program, you must first create the XM ASCII file "HPROJS" and enter an abbreviation for each project (make it 1 to 3 letters). One project per record in the file. The program will create a custom menu out of these project abbreviations, like "P1 P2 P3 P4", where each abbreviation corresponds to a local label (here A to D). In this example hours to the "P1" project is registered by pressing the A key (in User mode), while hours to the "P3" project is registered pressing C.

To register hours, run the program. The current date will be in the X register. If you want to register hours for another date, then enter that date (only month and day in the format that you have for your calculator - MDY or DMY; Example = Enter in the X register "25.04" for 25th of April if you have DMY as the format or "04.25" if MDY is your format). Enter the hours worked that day. Enter the description in Alpha and press the local label (A up to E) for the project you want to register hours for. The program shows you the record (truncated to 24 characters) that is added to the HOURSF file (the XM ASCII file where all hours entries are registered). If you have your HP-41 hooked to a PC via HP-IL, you may then download and extract all hours from HOURSF by using this solution: https://github.com/isene/HP-41CL_HOURS.rb

In addition to the dynamically created local labels A - E, pressing the local label "a" (or using the global label "PED") will let you edit the HPROJS file. Label "c" (or "HCLR") will clear (empty) the HOURSF file and "e" (or "HED") will let you edit the HOURSF file (in case you have misregistered something).

The program depends on the ISENE.ROM routines "SKPTACR", "FLSZ+" and "FLSZ-" (or you may just take those rotuines from the module).

## License
This software is released into the Public Domain.
