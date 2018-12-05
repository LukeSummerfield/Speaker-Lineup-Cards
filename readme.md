# Speaker Lineup Cards Module
This module is for showcasing upcoming speakers at an event. This module is meant to be used with a [Coded HubSpot Template](https://knowledge.hubspot.com/articles/kcs_article/cos-general/build-a-custom-coded-template-in-hubspot) as this utilzies [Bootstrap 4](https://getbootstrap.com/) in order to function. The following resources were used:
* https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css
* https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/js/bootstrap.min.js

A demo of this in action can be seen on the Chicago HubSpot User Group ChiX event page: http://chicago.hubspotusergroups.com/x

## How to use this module
After coding your custom template, your best use with this module inside of pre-defined Flexible Column area. You can create a Flexible Column Container using the `{% widget_container %}` tag. An example of this is below:

```
<!-- Section Wrapper for styling full-width -->
<section class="alt" id="speakers">
  <!-- Bootstrap .container -->
  <div class="container">
	
	<!-- Flexible Column widget_container -->
    {% widget_container "speaker_cards_row" label="Speaker Card Rows" %}
		<!-- Add the Speaker Lineup Card Moudle via the page editor -->
    {% end_widget_container %}

  </div>
</section>
```

Once you have this section in your template, you can simply add the Speaker Lineup Card Module through the page editor by using the left side `+` sign or by using the `Edit Module` button. See the Flexible Column section in this article for more information: https://knowledge.hubspot.com/website-user-guide/how-to-use-content-modules

## Features
The Speaker Lineup Cards make use of [repeating fields](https://designers.hubspot.com/docs/modules/repeating-fields-and-loops) and come with the following field options inside of each repeater group:

* Speaker Headshot (Image Field)
* Speaker Name and Title (Rich Text Field)
* Speaker Card Body Content (Rich Text Field)
* Speak Card Width (Number: Min 1 - Max 12)
* Page Field (Page Selector)

![Speaker Card Settings](https://raw.githubusercontent.com/ajlaporte/Speaker-Lineup-Cards/master/screenshots/3-speaker-card-settings.gif "Speaker Card Settings")

## Additional Screen Shots

Front Side View
![Speaker Row Cards ](https://raw.githubusercontent.com/ajlaporte/Speaker-Lineup-Cards/master/screenshots/2-speaker-row-cards.jpg "Speaker Row Cards")

DMv2 View
![DMv2 View ](https://raw.githubusercontent.com/ajlaporte/Speaker-Lineup-Cards/master/screenshots/1-behind-the-scenes.jpg "DMv2 View")
