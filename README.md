Drupal - YouTube Playlist Integration
==========================================

This is a simple make file that is to be used with <a href="http://drupal.org/project/drush_make">Drush Make</a> in
order to set the ground work of a YouTube playlist importer site within Drupal.  Here are the steps to follow to get 
this working.

- Install drush + drush make on your machine.
- Clone this repo into the docroot of your Local Machine or server.
- Change directories into the directory and type
  ```
    drush make youtube.make www
  ```
- Setup a VirtualHost to point to the www as the docroot for your site.
- Install Drupal as you normally would (with http://mysite.com/install.php)
- Walk through the installer.
- When you are done, go to Modules and enable the "MediaFront: YouTube Playlist Feeds" module.
- Now, create content - "YouTube Channel"
- Give your feed a title.
- Go to <a href="https://developers.google.com/youtube/2.0/developers_guide_protocol_video_feeds">YouTube API</a> to find a feed you wish to import, and put that in the FEED URL text field.
- Click save and it will import the whole feed into content into your site.
- Enjoy!!!