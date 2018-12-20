# Capture xMatters Instance Data (capture-instance-data.py)
A Python utility to capture as much xMatters Instance data as possible for use by the .  The script currently backs-up the following information:

   * Sites
   * Users
   * Devices with Timeframes
   * Groups
   * Shifts

The information is preserved in timestamped files so that you can run this via automation as often as you like.  If a catastropy does happen, you will have all of the information necessary to recover most of your environment by using the companion [Restore xMatters Instance Data](tbd) Utility.

 format of the information is made specifically to be used by The following A note about what the product is and what this integration/scriptlet is all about. Check out the sweet video [here](media/mysweetvideo.mov). Be sure to indicate what type of integration or enhancement you're building! (One-way or closed-loop integration? Script library? Feature update? Enhancement to an existing integration?)

<kbd>
  <img src="https://github.com/xmatters/xMatters-Labs/raw/master/media/disclaimer.png">
</kbd>

# Pre-Requisites
* Version 453 of App XYZ
* Account in Application ABC
* xMatters account - If you don't have one, [get one](https://www.xmatters.com)!

# Files
* [ExampleCommPlan.zip](ExampleCommPlan.zip) - This is an example comm plan to help get started. (If it doesn't make sense to have a full communication plan, then you can just use a couple javascript files like the one below.)
* [EmailMessageTemplate.html](EmailMessageTemplate.html) - This is an example HTML template for emails and push messages. 
* [FileA.js](FileA.js) - An example javascript file to be pasted into a Shared Library in the Integration builder. Note the comments

# How it works
Add some info here detailing the overall architecture and how the integration works. The more information you can add, the more helpful this sections becomes. For example: An action happens in Application XYZ which triggers the thingamajig to fire a REST API call to the xMatters inbound integration on the imported communication plan. The integration script then parses out the payload and builds an event and passes that to xMatters. 

# Installation
Details of the installation go here. 

## xMatters set up
1. Steps to create a new Shared Library or (in|out)bound integration or point them to the xMatters online help to cover specific steps; i.e., import a communication plan (link: http://help.xmatters.com/OnDemand/xmodwelcome/communicationplanbuilder/exportcommplan.htm)
2. Add this code to some place on what page:
   ```
   var items = [];
   items.push( { "stuff": "value"} );
   console.log( 'Do stuff' );
   ```


## Application ABC set up
Any specific steps for setting up the target application? The more precise you can be, the better!

Images are encouraged. Adding them is as easy as:
```
<kbd>
  <img src="media/cat-tax.png" width="200" height="400">
</kbd>
```

<kbd>
  <img src="media/cat-tax.png" width="200" height="400">
</kbd>


# Testing
Be specific. What should happen to make sure this code works? What would a user expect to see? 

# Troubleshooting
Optional section for how to troubleshoot. Especially anything in the source application that an xMatters developer might not know about, or specific areas in xMatters to look for details - like the Activity Stream? 
