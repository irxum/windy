# Readme

This repo will provide guidance for the wind project

# Big Goal
- Given a dataset, find a way to detect real high wind speed scenarios.
- With a method to detect real high wind speed scenarios, develop algorithm to predict them.

# User Scenario
I am a powerplant operator.  I have some special equipment in my powerplant.  It is designed only to function properly as long as the wind speed is below a certain value, let’s call that ‘x’.  I know it’s very possible that the wind speed can go above ‘x’ so I installed a special mechanism to protect my equipment in situations when the wind speed exceeds ‘x’.  But there’s a catch, it takes 'y’ minutes for the mechanism to fully protect the equipment.  So ideally, I’d like a way to predict when the wind speed would go above ‘x’ in the next ‘y’ minutes.  So if I had a nice prediction tool that sounded an alarm when the wind speed might exceed ‘x’ in the next ‘y’ minutes, that would really help me as a powerplant operator.  

# Challenges
- The wind speed data is not clean.  It will be important to remove time intervals that are obviously not use-able.  For example, there may be periods when the windspeed values are all NaN, blank or zero.
- Some wind speed data is clearly not real.  For example, some wind speeds recorded may be HIGHER than the world record for wind speeds.
- The wind speed data is large and organized in a manner that may not be conducive for what you want to do.  This is an opportunity to practice with AWS s3.  Try transferring a small amount of the data to an AWS s3 for further work / organization.


# Data Sources
One minute interval wind speed data is available here:
ftp://ftp.ncdc.noaa.gov/pub/data/asos-onemin/

Details for the wind data is found in:
ftp://ftp.ncdc.noaa.gov/pub/data/asos-onemin/td6405.txt

Information about weather stations is found here:
https://www.faa.gov/air_traffic/weather/asos/

General information about ASOS is here:
https://www.weather.gov/asos/



# Final Deliverable
The report and code should be captured in your own github.  There is no working around this requirement.  The report should be written as an .md file.  The code should be checked into github.
