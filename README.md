Front End Developer Assessment
==============================

As a Learner, I would like to easily switch between viewing 'Most Popular' and 'Upcoming' courses, in a small modular sidebar area on a page.

You should build a suitable page layout to accomodate this module in the sidebar, mobile first. In the mobile view, the module will wrap under main content and display at the bottom of the page. 

There is a JSON feed of 5 courses for each list available to provide the data. 

As a minimum, the lists should be numbered and link to the relevant course detail page on the FutureLearn site.

An enhancement to this would be to provide a modal overlay which would appear when a link is clicked providing an intro and synopsis before providing the user with a button to join that course.

The look and feel of the module should match the visuals provided in the `visuals' folder.

for additional guidance, you can use the FutureLearn styleguide at: https://www.futurelearn.com/styleguide

Copies of the JSON feeds are available in this repo but they are also hosted on JSONstub to prevent localhost domain AJAX security issues. You can access them like so;


'Most Popular' JSON feed using jQuery
-------------------------------------
    $.ajax({
        type: 'GET',
        url: 'http://jsonstub.com/courses/most-popular',
        beforeSend: function (request) {
            request.setRequestHeader('JsonStub-User-Key', '6f34b706-c669-40b0-bef7-21f183cdbf29');
            request.setRequestHeader('JsonStub-Project-Key', '8785ce43-d2f0-45b8-8ada-1e8d3d84bd83');
        }
    }).done(function (data) {
        //do something with data
    });




'Upcoming' JSON feed using jQuery
---------------------------------
    $.ajax({
        type: 'GET',
        url: 'http://jsonstub.com/courses/upcoming-courses',
        beforeSend: function (request) {
            request.setRequestHeader('JsonStub-User-Key', '6f34b706-c669-40b0-bef7-21f183cdbf29');
            request.setRequestHeader('JsonStub-Project-Key', '8785ce43-d2f0-45b8-8ada-1e8d3d84bd83');
        }
    }).done(function (data) {
        //do something with data
    });


Getting Started
---------------
Please clone this repo and push changes to branch with name of the candidate.


