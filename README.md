# demo-request-video-landing-page
Standard landing pages have marketing copy and a graphic on one side and a long form on the other side of the page. Filling out this form usually sends you some kind of marketing collateral, requests further information, or in our case, requests a demo. Giving a product demo every time someone fills out your landing page may not be logistically feasible so perhaps it's time to think outside of the box.  

By creating a demo video you can streamline your sales process, save money, and automate your lead generation initiatives. But where does the demo video go? You still want to capture prospect and lead information so just placing it on your website won't do. That's where this landing page design comes in. Not only does this design and functionality streamline your sales process, you still collect lead data, and you can give thousands of demos a minute without having to pool any internal resources to do so. Enjoy. 

In this tutorial, [Solodev](https://www.solodev.com/) will show you how to create a landing page with a demo video accessible after form submission.

# Tutorials

For detailed instructions, view Solodev's [Crafting a Request a Demo Landing Page with Video](https://www.solodev.com/blog/web-design/crafting-a-request-a-demo-landing-page-with-video.stml) article.

# Demo

Try out a working example on [JSFiddle](https://jsfiddle.net/solodev/zjeksj84/).

# HTML

The landing page contains the following basic HTML markup.

```
<section class="container">
   <div class="row">
      <div class="col-md-7">
         <h2 class="no-margin-top h1 center-small">See Solodev in action.</h2>
         <p class="bottom-pad">Solodev is an industry-leading web experience software solution that empowers organizations with total design freedom.</p>
         <div class="text-center overlaycontainer vimeo-video widescreen bottom-buffer">
            <div class="overlay">
               <p>COMPLETE THE FORM TO VIEW DEMO</p>
            </div>
            <div class="mboxDefault" style="visibility: visible; display: block; user-select: auto;">
               <iframe src="https://player.vimeo.com/video/205597179" width="500" height="281" frameborder="0" webkitallowfullscreen="" mozallowfullscreen="" allowfullscreen=""></iframe>
            </div>
         </div>
      </div>
      <div class="col-md-5">
         <div class="form-stacked shade-brand">
            <div data-track-position="requestademomasterform">
               <div class="master_form_container">
                  <form action="/" accept-charset="UTF-8" name="demo-request" class="validate-form" id="demo-request-form" novalidate="novalidate">
                     <div class="master_form inline-form">
                        <h3 class="no-margin">Fill out the form to get instant access to an exclusive video demo.</h3>
                        <div class="row">
                           <!--First Name-->
                           <div class="form-group col-sm-6">
                              <label for="first_name" class="control-label">First Name</label>
                              <input id="first_name" class="required form-control noSpace" title="Please enter your first name" placeholder="First Name" name="first_name" type="text" value="" aria-required="true">
                           </div>
                           <!--Last Name-->
                           <div class="form-group col-sm-6">
                              <label for="last_name" class="control-label">Last Name</label>
                              <input id="last_name" class="required form-control noSpace" title="Please enter your last name" placeholder="Last Name" name="last_name" type="text" value="" aria-required="true">
                           </div>
                        </div>
                        <div class="row">
                           <!--Business Email-->
                           <div class="form-group col-sm-6">
                              <label for="email" class="control-label">Business Email</label>
                              <input id="email" class="email required form-control" title="Please enter a valid email" placeholder="Business Email" autocomplete="off" name="email" type="email" value="" aria-required="true">
                           </div>
                           <!--Phone-->
                           <div class="form-group col-sm-6">
                              <label for="phone" class="control-label">Phone</label>
                              <input id="phone" class="phone required form-control" title="Please enter a valid phone number" placeholder="Phone" name="phone" type="tel" value="" aria-required="true">
                           </div>
                        </div>
                        <div class="row">
                           <!--Company-->
                           <div class="form-group col-sm-6">
                              <label for="company" class="control-label">Company</label>
                              <input id="company" class="required form-control" title="Please enter a valid company" placeholder="Company" autocomplete="off" name="company" type="text" value="" aria-required="true">
                           </div>
                           <div class="form-group col-sm-6">
                              <label for="title" class="control-label">Title</label>
                              <input id="title" class="required form-control" title="Please enter a valid job title" placeholder="Title" autocomplete="off" name="title" type="text" value="" aria-required="true">
                           </div>
                        </div>
                        <div class="row">
                           <div class="form-group col-sm-6">
                              <label for="department" class="control-label">Department</label>
                              <select id="department" title="Please enter a valid department" class="required form-control" name="department" aria-required="true">
                                 <option value="" selected="selected">Department</option>
                                 <option value="CEO/C-Suite">CEO</option>
                                 <option value="Customer Service and Support">Customer Service</option>
                                 <option value="Engineering/Product Development">Product Development</option>
                                 <option value="Finance">Finance</option>
                                 <option value="HR">HR</option>
                                 <option value="IT">IT</option>
                                 <option value="Marketing">Marketing</option>
                                 <option value="Operations">Operations</option>
                                 <option value="Sales and Business Development">Business Development</option>
                                 <option value="Other">Other</option>
                              </select>
                           </div>
                           <div class="form-group col-sm-12">
                              <label class="show auto-demo-checkbox"><input id="autoDemoCheckbox" checked="checked" name="custom_demo_request" type="checkbox" value="1">&nbsp;&nbsp; Customize your demo. </label>
                           </div>
                           <div class="form-group col-sm-6 top-buffer mainformsubmit">
                              <div class="mboxDefault" style="visibility: visible; display: block; user-select: auto;">
                                 <button class="btn btn-primary" id="masterformsubmit" href="/">Watch Now</button>
                              </div>
                           </div>
                        </div>
                     </div>
                  </form>
               </div>
            </div>
         </div>
      </div>
   </div>
</section>
```

# CSS

All required CSS is in video-demo-lp.css

# External Includes

This tutorial includes the following third party resources.

```
<link href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" rel="stylesheet">
<link href="video-demo-lp.css" rel="stylesheet">
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.1/jquery.min.js"></script>
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
```
