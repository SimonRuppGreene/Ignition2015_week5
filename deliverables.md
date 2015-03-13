#### Deliverables for week 5 Rails MVC
##### Odin Project Routing Guide Questions:
- What is the "Root" route?
  - The action that maps to the base URL for the website
- What are the seven RESTful routes for a resource?
  - index, show, new, create, edit, update, destroy
- Which RESTful routes share the same URL but use different verbs?
  - (index, create), (show, update, delete) 
- How do you specify an ID or other variable in a route?
  - ":[variable_name]", which is then accessed through the params hash
- How can you easily write all seven RESTful routes in Rails?
  - put "resources :[controller_to_route]" in config/routes.rb
- What is the Rails helper method that creates the HTML for links?
  - "link_to 'display text', [path]"

##### Odin Project Views Guide Questions:
- What is a layout?
  - a layout is the shell of the actual content of a webpage, it contains html that's present across the entire website like     html, head, body tags and the footer and header of the website
- What's the difference between a "view template" and a "layout"?
  - a view template is the file that contains the html that gets inserted into the layout when a certain action is               called/page is rendered
- What is a "Preprocessor"?
  - a preprocessor is a program that parses a file and converts embedded preprocessor statements into another language, like     html, javascript, or css
- Why are preprocessors useful?
  - preprocessors allow for dynamic and programmatic generation of html elements in a convenient fashion, such as looping        through all of one's blog posts and inserting the data into a repeatedly used template or view partial instead of doing      it by hand
- How do you make sure a preprocessor runs on your file?
  - make sure one has the right extensions to tell the preprocessor to run, have the right gems installed, and i think           there's some config files for the app that have to be set somewhere, i was having issues with css preprocessing on a         previous assignment until i changed a config option but i don't remember which one 
- What's the outputted filetype of a preprocessed *.html.erb file? What about a *.css.scss file?
  - *.html.erb file => *.html file, *.css.scss file => *.css file
- What is the difference between the <%= and <% tags?
  - <%= renders the output of the contained statement, <% does not
- What is a view partial?
  - a piece of html that's reused in different areas of one's application, designated by a leading underscore
- How do you insert a partial into your view?
  - pass the name of the partial to render, sans leading underscore
- How can you tell that a view file is a partial?
  - the file has a leading underscore in its name
- How do you pass a local variable to a partial?
  - pass a hash containing the local variables desired to the partial when rendering
- What's the magical Rails shortcut for rendering a User? A bunch of Users?
  - rendering the user object directly: <%= @users.each do |user| render user %> or
  - <%= render @users %>
- What are asset tags and why are they used?
  - the tags that are used to insert javascript, css, and image assets into a web page, the helper methods
    are provided as a convenience in generating the whole html tag for you as well as locating the file itself 
    so its less likely that one will break something through typing a path incorrectly
  

##### Link to Odin Project Basic Routes, Views and Controllers repo: [my odin repo](<https://github.com/SimonRuppGreene/ignition-week5-c9>)
##### Link to Hartl's Rails Tutorial Chapter 5 repo: [my hartl's repo](<https://github.com/SimonRuppGreene/rails-tutorial>)
