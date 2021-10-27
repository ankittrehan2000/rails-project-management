# README

A very basic project management application built with rails and bootstrap

Learning Notes:

`<%= yield %>` tag can be replaced by a chunk of html code

A scaffold in rails is a full set of model, database migrations, views and controllers

`@variable` is an instance variable that is defined inside of a controller which is accessible by views

`current_user` is a method provided by the Devise auth framework

`rails generate (g) home index` creates a home model and an index file

Routes.rb - `home/get` maps to a method in the home controller

While outputting `<%= %>` but if we need to loop or do something else dynamic use `<% %>`

Use `<%= render 'home/header' %>` to render partial with name _home.html.erb

`<%= link_to 'Name of link', root_path/home_about_path, class:"" %>` for linking in rails apps where home_about_path is the path that routes to the home controller with about method

`rails g scaffold Friend first_name last_name:string` is like creating a database table with the columns first_name and last_name. This also generates models, views, and controllers

`resources :friends` means that rails knows to create all the CRUD routes for friends

`rails generate devise MODEL` creates a table to store the user data

`class_params` method lists all the allowed parameters for creating

Under the hood rails uses `pluralize` in order to create a database table and to know where to look when dealing with an instance of that model.
