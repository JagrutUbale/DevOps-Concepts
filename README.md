##Concepts


<ol>
<br>
<li> In your own words, explain the difference between continuous integration, continuous delivery, and continuous deployment.</li>

<u><b>Answer</b></u>
<ul>
<li><u>Continuous Integration</u> <br>
Continuous Integration can be defined as practice where developers automatically build, test, and analyze a software change in response to every software change committed to the source repository.<br>
<i>It is also a strategy for how a developer can integrate code to the mainline continuously - as opposed to frequently</i></li>
<li><u>Continuous Delivery</u> <br>
Continuous Delivery is described as the <b><i>logical evolution</i> of continuous integration</b><br> Always be able to put a product into production!<br>
So, it can be defined as a practice that ensures that a software change can be delivered and be ready for use by a customer by testing in <b>production-like</b> environments.
<li><u>Continuous Deployment</u> <br>
Continuous Deployment can defined as a practice where incremental software changes are automatically tested, vetted, and deployed to production environments.<br>
<b>Automatically deploy the product into production whenever it passes QA!</b><br>
<a href="http://stackoverflow.com/questions/28608015/continuous-integration-vs-continuous-delivery-vs-continuous-deployment">Source</a>

</ul>
<br>
<li>How does DevOps team model (e.g., site reliability engineer) differ than a NoOps team model (e.g. Netflix team)? What differences in architecture allow for a NoOps model?</li>
<ul><br>

<li>With the rise in DevOps, it becoming pretty common beleif that if development teams can be empowered to move things from test and development and into operations, then why not make them responsible for maintaining that code in the production environment? This is giving rise to NoOps, in which complete automation of the development to operational process takes place.
<br>

<u><b>Answer</b></u>

In DevOps, reliability engineers are responsible for all of their work from testing to staging. <b>By owning
a feature or code change from
cradle to grave (from inception to
deployment)</b>, the burden is on the
developer. This burden means that
when things break, the developer
is the one who gets the support call
and must fix the issue, no matter
what time of day. "You are the Support person". That is, developers have the power and freedom to deploy changes at their own behest.<br>
<u><strong>Netflix has no dedicated operations teams</strong></u> But all the other roles such as the QA and the developers etc, they’re embedded in the development teams.<br><br>
<u><b>Architectural changes</b></u> <br>
<li>Netflix achieves this integration through a microservices architecture that requires teams to build APIs that they maintain and ensure are stable from change to change.</li>
<li>Google enforces team service communication through a common API type and a defined data type that all services must use.</li>
<li>With defined communication standards, teams are free to build what they need to accomplish their tasks, in whatever way is the most efficient for them.</li>

</ul>
<br>
<li>Explain the principle of "Every Feature is an Expertiment"
	<br>
	<b><u>Answer</u></b>
	<ul>
	<li>
	Every Feature is an Expertiment is one of The Top 10 Adages in Continuous Deployment. With continuous deployment, developers treat every planned feature as an experiment, allowing some deployed features to die.
	</li>
	<li>For example, on Netflix.com, if not enough people hover over a new element, a new experiment might move the element to a new location on the screen.</li>
	<li>
	Generally, the companies collect statistics
on every aspect of the software. However, there are challenges associated to it too.<br> For example, Netflix initially collected 1.2 million metrics related to its streaming services, but that soon ballooned to 1 billion metrics. Not only could the in-memory data store no longer keep up, but the company also had to more carefully consider what data was essential for experimentation
	</li>
	
	</ul>

</li>
<br>
<li>Explain the principle of Be Fast to Deploy, Slow(er) to Release.</li>
<b><u>Answer</u></b>
<ul>
<li>Every company nowadays is using or planning on using Continuous Deployment strategies to increase their speed, efficiency and availability of product in the market. However, this always is not the case .
<br>Deploying code into production doesn’t necessarily mean user-facing features are available to customers right away. Sometimes, a new feature might be deployed and evaluated during production for several months before being publicly released.
</li>
<li>Many organizations hence are using Dark Launches. <br><b>Dark launching</b> practice is the one in which code is incrementally deployed into production but remains invisible to users.<br>This dark launch lets the engineer slowly deploy and stabilize small chunks directly during production without impacting the user experience. After stabilization, the engineer can turn on the feature and release it.</li>
<li> <b>Example:</b>
 Microsoft often deploys large architectural changes, using a combination of dark launches and feature flags. With a feature flag, a feature is deployed but disabled until it’s ready for release. The developer turns the feature off and on through a configuration server.
<li>
<b>Important</b>: Companies must spend extra engineering effort to ensure that delayed-release strategies and testing during production don’t negatively affect the user experience.
</li>

</ul>
</ol>





##Git Hooks

   * The link to the hook Script can be found here
      
	 [LINK to hook file ](https://github.ncsu.edu/vbhat/HW0/blob/master/resources/post-commit)



##Screencast

* [Sreencast](https://youtu.be/pOWYzFxqKT4)





