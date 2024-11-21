<H2>Cloud Architecture</H2>
<H4>Objective</H4>
<P>The objective of this first assignment is to demonstrate the deployment and automated
management of a load-balanced auto-scaling web application</P> </br>
<h4>Core functionality specification</h4>
<ol>
  <li>Creation and configuration of a “master” instance of a web application. You may choose any
web application, ideally one that relies on a third party or backend service. Note: any
backend services/databases chosen should require just low cost resources. At a minimum
you should implement auto-scaling of the application server and discuss issues relating to
the scaling of a backend if you don't implement one. </li>
  <li>Creation of a custom AMI based on your master instance, to be used by EC2 auto-scaling
within a VPC infrastructure. </li>
<li>Creation of a VPC with subnets into which your application will be deployed. You are required
to deploy the final version of your architecture with target instances in private subnets. We
recommend that you use public subnets when testing your configuration and move to private</li>
<li>Creation of an application load balancer with a HTTP (or HTTPS) listener. Creation of a
launch template based on your custom AMI. Creation of an auto-scaling group based on
your launch template and linked to your load balancer.</li>
<li>Configuration of dynamic scaling policies (using simple or step scaling) based on
CloudWatch alarms to cause an increase in resources when required and also a decrease in
resources when conditions return to normal. You should configure scaling based on one or
more metrics other than solely CPU utilisation – a combination of metrics including CPU
utilisation is acceptable. You must justify your choice of metric(s) in your report.</li>
<li>Generation of test traffic to the load balancer – e.g. using curl/wget or a web testing tool.</li>
<li>Demonstrate load balancing in action – i.e. show that it is distributing the traffic across
multiple target web servers – e.g. by viewing individual web server logs or other logs such as
load balancer logs. Include screenshots and a brief explanation in your report.</li>
<li>Use of your own script to monitor custom metrics on your servers and push these to
CloudWatch. For example this could be web server or other server logs, or OS activity (CPU,
memory, disk, number of processes, etc).</li>  
</ol>  

<h4>Additional functionality</h4>
<ol>
  <li> AWS Key Managment system for encryption or any file</li>
  <li>Automate the basic specification, or part of it, using the AWS SDK – e.g. Python/boto.</li>
</ol>




