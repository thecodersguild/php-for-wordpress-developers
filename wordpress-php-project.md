# WordPress PHP Project

- Create a plugin called 'My Events'
- Create an 'Event' post type
- Create an 'Event Details' meta box
- Add an 'Address' field to the meta box (field name should be geo_address)
- Save the field data when the user clicks the 'Update' button
- On save, send the address to the Google Geocoding API to fetch the coordinates. (http://maps.googleapis.com/maps/api/geocode/json?address=<address_field>)
- Store geo-coordinates as post meta according to the WordPress standards (https://codex.wordpress.org/Geodata)
- Add a filter for the content to output the address and coordinates before the content
- Add a filter to post type args to customize the post type slug