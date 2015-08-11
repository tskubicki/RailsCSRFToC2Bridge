# RailsCSRFToC2Bridge (Rails CSRF Token to Construct 2 Bridge)

A simple Construct 2 plugin that allows a project to be able to POST a Rails setup that utilizes CSRF protections. 
Pulls the CSRF token from Rails for use in POSTing(Can't verify CSRF token authenticity)

To use:
- Clone this repo to your "Construct 2\exporters\html5\plugins" folder.
- Add the object "RailsCSRFToC2Bridge" in your project
- Use its expression "RailsCSRFToC2Bridge.getCSRFToken", contained in a URLEncode(). 
 An example:
  '''score="&player_score&"&authenticity_token="&URLEncode(RailsCSRFToC2Bridge.getCSRFToken)'''
