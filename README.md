Salesforce Marketing Cloud Servers are in Guatemala Country hence system time will be Guatemala City time. Time Difference between Guatemala City, Guatemala and Melbourne/Sydney, Australia is varying. 
* 16 Hours Difference During Standard Time - AEST (April to October) 
* 17 Hours Difference During Daylight Savings Time - AEDT (October to April)  

**Problem:**
We don’t have the standard functionality (in SQL) which consider above difference and converts the SFMC system time to Melbourne/Sydney time without any difference.

Why do we need to convert the time?
As explained above Salesforce Marketing Cloud server’s Date & Time is in different time zone, converting to local time is very important  factor which worries our development team a lot. Some of the scenarios where we required time conversions are:
* Custom Campaign ReportingCancel changes
* Extracting Tracking Data
* Date Comparison Conditions for Journeys
* Use for “Wait By Attribute” in Journeys
* Datetime stamp for contact record addition/ updating in SFMC.

**Solution:**
Finding the offset difference between each Time zone and calculating the total difference hours from Guatemala City, Guatemala Country to Sydney City, Australia.


