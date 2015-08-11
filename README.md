# RailsCSRFToC2Bridge (Rails CSRF Token to Construct 2 Bridge)

A simple plugin that allows a Construct 2 project to be able to POST a Rails setup that utilizes CSRF protections. 
Pulls the CSRF token from Rails for use in POSTing(Can't verify CSRF token authenticity)

To use:
- Clone this repo to your "Construct 2\exporters\html5\plugins" folder.
- Add the object "RailsCSRFToC2Bridge" in your project
- Use its expression "RailsCSRFToC2Bridge.getCSRFToken", which returns the CSRF
  token in Rails' <% csrf_meta_tags %> helper. An example:
  '''score="&player_score&"&authenticity_token="&RailsCSRFToC2Bridge.getCSRFToken'''
