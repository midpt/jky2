---
layout: default
title: Hello World!
tagline: Supporting tagline
---
{% include JB/setup %}

Read [Jekyll Quick Start](http://jekyllbootstrap.com/usage/jekyll-quick-start.html)

Complete usage and documentation available at: [Jekyll Bootstrap](http://jekyllbootstrap.com)



## My own paragraph

----------------
Classic Bootstrap Components

  <h3>Button Styles</h3>
  <button type="button" class="btn btn-default" onclick="javascript: alert('Default')">Default</button>
  <button type="button" class="btn btn-primary" onclick="javascript: alert('Primary')">Primary</button>
  <button type="button" class="btn btn-success" onclick="javascript: alert('Success')">Success</button>
  <button type="button" class="btn btn-info" onclick="javascript: alert('Hello')">Info</button>
  <button type="button" class="btn btn-warning" onclick="javascript: alert('Hello')">Warning</button>
  <button type="button" class="btn btn-danger" onclick="javascript: alert('Danger')">Danger</button>
  <button type="button" class="btn btn-link"  onclick="javascript: alert('Link')">Link</button>      


  <h3>Alerts</h3>
  <div class="alert alert-success">
    <strong>Success!</strong> This alert box could indicate a successful or positive action.
  </div>
  <div class="alert alert-info">
    <strong>Info!</strong> This alert box could indicate a neutral informative change or action.
  </div>
  <div class="alert alert-warning">
    <strong>Warning!</strong> This alert box could indicate a warning that might need attention.
  </div>
  <div class="alert alert-danger">
    <strong>Danger!</strong> This alert box could indicate a dangerous or potentially negative action.
  </div>
  
  

  <h3>Modal Example</h3>
  <!-- Trigger the modal with a button -->
  <button type="button" class="btn btn-info btn-lg" data-toggle="modal" data-target="#myModal">Open Modal</button>

  <!-- Modal -->
  <div class="modal fade" id="myModal" role="dialog">
    <div class="modal-dialog">
    
      <!-- Modal content-->
      <div class="modal-content">
        <div class="modal-header">
          <button type="button" class="close" data-dismiss="modal">&times;</button>
          <h4 class="modal-title">Modal Header</h4>
        </div>
        <div class="modal-body">
          <p>Some text in the modal.</p>
        </div>
        <div class="modal-footer">
          <button type="button" class="btn btn-default" data-dismiss="modal">Close</button>
        </div>
      </div>    
    </div>
  </div>
 
  <h3>Dropdowns</h3>
  <p>The .dropdown class is used to indicate a dropdown menu.</p>
  <p>Use the .dropdown-menu class to actually build the dropdown menu.</p>
  <p>To open the dropdown menu, use a button or a link with a class of .dropdown-toggle and data-toggle="dropdown".</p>                                          
  <div class="dropdown">
    <button class="btn btn-primary dropdown-toggle" type="button" data-toggle="dropdown">Dropdown Example
    <span class="caret"></span></button>
    <ul class="dropdown-menu">
      <li><a href="#">HTML</a></li>
      <li><a href="#">CSS</a></li>
      <li><a href="#">JavaScript</a></li>
    </ul>
  </div> 

   <h3>Jumbotron</h3>
   <div class="jumbotron">
    <h4>Bootstrap Tutorial</h4>      
    <p>Bootstrap is the most popular HTML, CSS, and JS framework for developing responsive, mobile-first projects on the web.</p>
  </div>
    

 <!--   Image carousel                        -->
 <h3>Image Carousel</h3>
  <br/>
  <div id="myCarousel" class="carousel slide" data-ride="carousel">
    <!-- Indicators -->
    <ol class="carousel-indicators">
      <li data-target="#myCarousel" data-slide-to="0" class="active"></li>
      <li data-target="#myCarousel" data-slide-to="1"></li>
      <li data-target="#myCarousel" data-slide-to="2"></li>
      <li data-target="#myCarousel" data-slide-to="3"></li>
    </ol>

    <!-- Wrapper for slides -->
    <div class="carousel-inner" role="listbox">
      <div class="item active">
        <img src="http://www.w3schools.com/bootstrap/img_chania.jpg" alt="Chania" width="460" height="345">
      </div>

      <div class="item">
        <img src="http://www.w3schools.com/bootstrap/img_chania2.jpg" alt="Chania" width="460" height="345">
      </div>
    
      <div class="item">
        <img src="http://www.w3schools.com/bootstrap/img_flower.jpg" alt="Flower" width="460" height="345">
      </div>

      <div class="item">
        <img src="http://www.w3schools.com/bootstrap/img_flower2.jpg" alt="Flower" width="460" height="345">
      </div>
    </div>

    <!-- Left and right controls -->
    <a class="left carousel-control" href="#myCarousel" role="button" data-slide="prev">
      <span class="glyphicon glyphicon-chevron-left" aria-hidden="true"></span>
      <span class="sr-only">Previous</span>
    </a>
    <a class="right carousel-control" href="#myCarousel" role="button" data-slide="next">
      <span class="glyphicon glyphicon-chevron-right" aria-hidden="true"></span>
      <span class="sr-only">Next</span>
    </a>
  </div>   
 <!--  End Image carousel                        -->

  <h3>Table - Contextual Classes</h3>
         
  <table class="table">
    <thead>
      <tr>
        <th>Firstname</th>
        <th>Lastname</th>
        <th>Email</th>
      </tr>
    </thead>
    <tbody>
      <tr class="success">
        <td>John</td>
        <td>Doe</td>
        <td>john@example.com</td>
      </tr>
      <tr class="danger">
        <td>Mary</td>
        <td>Moe</td>
        <td>mary@example.com</td>
      </tr>
      <tr class="info">
        <td>July</td>
        <td>Dooley</td>
        <td>july@example.com</td>
      </tr>
    </tbody>
  </table>
 

  <h3>Tooltip Example</h3>
  <a href="#" data-toggle="tooltip" title="Hooray!">Hover over me</a>


	<script>
	$(document).ready(function(){
		$('[data-toggle="tooltip"]').tooltip();   
	});
	</script>
 
----------------- 

## My site.pages listing

{% for page in site.pages %}
     Page path: {{page.path}}
	 Page url: {{page.url}}
	 Page categories: {{page.categories}}
     Page title: <p>{{page.title}}</p>
     Page description: <p>{{page.description}}</p>  
{% endfor %}
----------------------------

**Try table of content**

[TOC]


**Try with block quote**

>  This is block quote
>  Another line 
>  Last line

**Fence code **

```
Firse line of fence code
Another line
Last line
```




## Update Author Attributes

In `_config.yml` remember to specify your own data:
    
    title : My Blog =)
    
    author :
      name : Name Lastname
      email : blah@email.test
      github : username
      twitter : username

The theme should reference these variables whenever needed.
    
## Sample Posts

This blog contains sample posts which help stage pages and blog data.
When you don't need the samples anymore just delete the `_posts/core-samples` folder.

    $ rm -rf _posts/core-samples

Here's a sample "posts list".

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

## To-Do

This theme is still unfinished. If you'd like to be added as a contributor, [please fork](http://github.com/plusjade/jekyll-bootstrap)!
We need to clean up the themes, make theme usage guides with theme-specific markup examples.


