---
layout: post
title: A Standard Login Screen & Best Practices
category: Web Design
tags: Security
---

<div class="row">
	<div class="span3 columns">
	  <br/>
	  <h3>Topic buzz</h3>
	  <p>What others are thinking. Add to the conversation and generate some chatter.</p>
	  <p><a href="https://twitter.com/share" class="twitter-share-button" data-via="leighvl">Tweet</a></p>
	  <p><g:plusone size="medium"></g:plusone></p>	
	  <p><script type="text/javascript" src="http://www.reddit.com/buttonlite.js?i=2&styled=off&url={{ page.url }}&newwindow=1"></script></p> 	  
	  <br/>
	  <h3>Read later</h3>
	  <p><a href="http://www.instapaper.com/hello2?url={{ page.url }}&title={{ page.title }}" title="Save {{ page.title }} to Instapaper" target="_blank">Save this blog post</a> for a later read or point of reference.</p>
    </div>
	<div class="span9 columns">
	  <br>
	  <p>When designing a standard Web Portal / Application for business use, there should be at least three main considerations that should be observed in order for the Application to be considered successful:</p>  
      <ul>
        <li>Stability</li>
        <li>Straightforwardness of use</li>
        <li>Security</li>
      </ul>
      <br>
      <p>While the first one is mighty obvious (if the web application doesn’t work, what purpose does it serve?) and may be discussed in future posts in further detail, the purpose of this post is to discuss the two other S’s one should consider in Web Form design; Straightforwardness & Security, and how by giving these priority ensure the former as well. </p>
      <br>
      <p>For a practical example, I chose to look at a regularly found screen on a web page designed for business use: the Login Screen.   Look below at a login screen, which I designed currently for my employer's Facilities Management System.</p>
	  <hr>
      <img src="/img/Login_Screen.png" alt ="Login Screen"></img>
	  <hr>
      <p>There we go… this page is laid out pretty simple, doesn’t it? For a login screen, this is as straight to the point as you can really get without causing the user unnecessary confusion, while at the same time, providing a basic standard of access into a web application. Notice there are really 3 main elements of this web form;</p>
      <ol>
        <li>A User Name textbox</li>
        <li>A Password Textbox</li>
        <li>A Confirm Button</li>
      </ol>
      <br>
      <hr>
      <h3>Straightforwardness</h3>
      <br>
      <p>The limiting of page elements to a select few to page area helps give the web form a feel of proper organization, while at the same time, effectively simplifying the website for the user. This concept of less on the website being more is very convenient to both the user and developer as this <em>minimalistic</em> approach will make the web app simple and easy to understand for the user, as well as help reduce the amount of data requested from the website to the browser, thus increasing page load times</p>
      <br>
      <hr>
      <h3>Security*</h3>
      <p>*<em>This is the consideration that really makes or breaks a functional web app in the long run IMO. So Please forgive my rambling</em>
      </p>
      <br>
      <p>The main function of a login screen on a web app is to provide a form of user authentication to regulate access to other parts of the web app. By providing a ‘Username’ and a ‘Password’ that match, the page will validate the user with the data provided and grant them continued access to the web app’s pages (which will be different dependent on the level of access for the user). </p>
      <br>
      <p>Besides making the overall web application secure from unauthorized intrusion by hackers and other unwanted persons, Security also encompasses fortifying the code used to create the web page itself and other server side scripting which is run which is necessary for the end usage of the site.</p>
      <br>
      <p>As this Login page is already minimal in nature (Fortunately) , there is not much work to be done in order to harden the page from the ‘usual exploits’, such as the ones listed below.</p>
      <ol>
      <li>SQL Injection</li>
      <li>Cross Site Scripting (XSS)</li>
      </ol>
      <br>
      <p>N.B.: No definition for these exploits will be given on this post (check related articles below or your friendly neighborhood Google if you are interested in more information). </p>
      <br>
      <p>But one fact to note about the ‘usual exploits’ is that these attacks require the injection of harmful code into the web page, resulting in an adverse effect to the page’s functionality.</p>
      <br>
      <p>Because of this, responsibility is really on the developer to prevent these exploits from occurring, by ensuring proper form validation is carry out on the user input before moving to another page, as well as ‘escaping’ any user entered characters, so that the user input is not treated as an operator in the web site’s scripting.</p>
	  <hr>
      <h2>Related Articles / Sources</h2>
      <br>
      
      <h5><a href="http://uxdesign.smashingmagazine.com/2011/05/05/innovative-techniques-to-simplify-signups-and-logins/" target="_blank">Innovated Techniques to Simplify Sign Ups & Login Pages</a></h5>
      <br>
      <h5><a href="https://www.owasp.org/index.php/XSS_(Cross_Site_Scripting)_Prevention_Cheat_Sheet" target="_blank">XSS Cheat Sheet</a></h5>
      <br>
      <h5><a href="https://www.owasp.org/index.php/SQL_Injection_Prevention_Cheat_Sheet" target="_blank">SQL Injection Cheat Sheet</a></h5>
     </div>
</div>

<div class="row">
	<div class="span3 columns">&nbsp;</div>
	<div class="span9 column">
			<p class="pull-right">{% if page.previous.url %} <a href="{{page.previous.url}}" title="Previous Post: {{page.previous.title}}"><i class="icon-chevron-left"></i></a> 	{% endif %}   {% if page.next.url %} 	<a href="{{page.next.url}}" title="Next Post: {{page.next.title}}"><i class="icon-chevron-right"></i></a> 	{% endif %} </p>  
	</div>
</div>

<div class="row">
	<div class="span3 columns">&nbsp;</div>
    <div class="span9 columns">     
		<h2>Comments Section</h2>
	    <p>Leave your thoughts and opinions on security in the comment section.</p>
		<div id="disqus_thread"></div>
		<script type="text/javascript">
			/* * * CONFIGURATION VARIABLES: EDIT BEFORE PASTING INTO YOUR WEBPAGE * * */
			var disqus_shortname = 'leighvl'; // required: replace example with your forum shortname

			/* * * DON'T EDIT BELOW THIS LINE * * */
			(function() {
				var dsq = document.createElement('script'); dsq.type = 'text/javascript'; dsq.async = true;
				dsq.src = 'http://' + disqus_shortname + '.disqus.com/embed.js';
				(document.getElementsByTagName('head')[0] || document.getElementsByTagName('body')[0]).appendChild(dsq);
			})();
		</script>
		<noscript>Please enable JavaScript to view the <a href="http://disqus.com/?ref_noscript">comments powered by Disqus.</a></noscript>
		<a href="http://disqus.com" class="dsq-brlink">blog comments powered by <span class="logo-disqus">Disqus</span></a>
	</div>
</div>

<!-- Twitter -->
<script>!function(d,s,id){var js,fjs=d.getElementsByTagName(s)[0];if(!d.getElementById(id)){js=d.createElement(s);js.id=id;js.src="//platform.twitter.com/widgets.js";fjs.parentNode.insertBefore(js,fjs);}}(document,"script","twitter-wjs");</script>

<!-- Google + -->
<script type="text/javascript">
  (function() {
    var po = document.createElement('script'); po.type = 'text/javascript'; po.async = true;
    po.src = 'https://apis.google.com/js/plusone.js';
    var s = document.getElementsByTagName('script')[0]; s.parentNode.insertBefore(po, s);
  })();
</script>