<!DOCTYPE html>
<html lang="en">

<head>
<META NAME="Author" CONTENT="Kamen">
</head>

<body>
<center>
<font face="Tahoma,Veradana" size="+3">
  Software for fast and accurate evaluation <br> of geomagnetic quantities at scattered points in space <br>
</font>
<font face="Courier New" size="+3">
  emmsynth_fast
</font>
</center>

<font face="Times" size="+0">
<font size="+2">
<p> <p> Overview
</font>

<p> We present FORTRAN and MATLAB software for fast and accurate evaluation of
the components of the geomagnetic field represented in high degree (above 720) solid spherical or ellipsoidal harmonics
at many scattered points in the space above the surface of the Earth.

<p> The evaluated magnetic field components are:
<ul> 
<li> North component in geocentric coordinates (in nT 'nanoTesla')
<li> East component in geocentric coordinates (in nT)
<li> Down component in geocentric coordinates (in nT)
<li> North component in geodetic coordinates (in nT)
<li> East component in geodetic coordinates  (in nT)
<li> Down component in geodetic coordinates (in nT)
<li> Horizontal intensity (in nT)
<li> Total intensity (in nT)
<li> Inclination (in decimal degrees)
<li> Declination (in decimal degrees)
</ul> 
The values of the components are derived from the official NOAA Enhanced Magnetic Models EMM2015 or EMM2017.
These models are determined by their coefficients, given 
in the files <font face="Courier New">EMM2015.COF</font> and <font face="Courier New">EMM2015SV.COF</font> for EMM2015 and
in the files <font face="Courier New">EMM2017.COF</font> and <font face="Courier New">EMM2017SV.COF</font> for EMM2017.

<p> The standard algorithm for evaluation of the above magnetic field components is relatively slow due to the high degree of the EMM.
Our algorithm performs several hundred times faster than the standard algorithm and evaluate every quantity with a guaranteed accuracy of less than 1 nT.

<p> The codes evaluate the magnetic field at millions of points given by their geodetic geographic coordinates:
latitude, longitude and the height above the Earth reference ellipsoid.
The height ranges from -0.417 km to 1,000 km. 

<p>
<font size="+2">
<p> Resources
</font>

<p> This is the GitHub
repository of <font face="Courier New">emmsynth_fast</font> source code, including instructions for compiling
and installing it. 
The FORTRAN version of the code is contained in the zip archive <a href="./emmsynth_fast_f.zip"><font face="Courier New">emmsynth_fast_f.zip</font></a> (32MB),
while the MATLAB version of the code is contained in the zip archive <a href="./emmsynth_fast_m.zip"><font face="Courier New">emmsynth_fast_m.zip</font></a> (32MB).

<p> Every zip file contains the respective source codes, the model coefficients, test files with coordinates of randomly distributed points in space,
the code output for these points and a user manual file <font face="Courier New">readme_emmsynth_fast.pdf</font>.
These user manuals contain a detailed description of the software with instructions for its use and test statistics.

<p> The  homepage for <font face="Courier New">emmsynth_fast</font> project can be found at 
<a href="http://imi.cas.sc.edu/sw-geomagnetic-fields/"><font face="Courier New">http://imi.cas.sc.edu/sw-geomagnetic-fields/</font></a>
from the University of South Carolina website.

</font>
</body>
</html> 