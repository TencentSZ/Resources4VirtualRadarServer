# Brief guide to Virtual Radar Sever

Virtual Radar Server is an open-source .NET application that runs a local web server. See https://www.virtualradarserver.co.uk/

This application writes data into and reads from its SQLite-formated database (take BaseStation.sqb for example)  with Database Writer Plugin. You can find the path in the options menu and open it with any database management tool you are familiar with.

If you query the table 'Aircraft' and luckily find the strings in OperationFlagCode field are the same as the bitmap filename in OperatorFlags directionary of this project, you can copy all the bitmap file into your local flags folder as is set in the options menu.

# Which type of flags is  included?

I am using Virtual Radar Sercer 2.4.4.36598 and after creating an empty database by Database Writer Plugin I found strings in OperatorFlagCode are 3-chars, like NCR, FDX and so on.

I checked out this repo    https://github.com/rikgale/VRSOperatorFlags , removed all bitmap filenames longer than 3 characters, and add some operator flags from Asian airlines.