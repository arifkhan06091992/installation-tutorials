# What is heroku ?
__Heroku is a cloud platform as a service__. That means you do not have to worry about infrastructure; you just focus on your application.

In addition to what Jonny said, there are a few features of Heroku:

- Instant Deployment with Git push - build of your application is performed by Heroku using your build scripts
- Plenty of Add-on resources (applications, databases etc.)
- Processes scaling - independent scaling for each component of your app without affecting functionality and performance
- Isolation - each process (aka dyno) is completely isolated from each other
- Full Logging and Visibility - easy access to all logging output from every component of your app and each process (dyno)

Heroku provides very well written tutorial which allows you to start in minutes. Also they provide first 750 computation hours free of charge which means you can have one processes (aka Dyno) at no cost. Also performance is very good e.g. simple web application written in node.js can handle around 60 - 70 requests per second.

Heroku competitors are:

- OpenShift by Red Hat
- Windows Azure
- Amazon Web Services
- Google App Engine
- VMware
- HP Cloud Services
- Force.com

## Heroku vs. AWS: Which Is Best for Your Startup?
Amazon Web Services (AWS) and Heroku are two commonly used cloud services that let us deploy, monitor, and scale web and mobile applications. Both services provide us with cloud computing resources and are great for hosting applications. But if you’re building your first mobile or web application, how can you decide which of these options — AWS or Heroku — is best for your application?

Choosing a hosting service becomes even harder when we take a glance at the number of products AWS offers. It’s easy to get lost.

### Heroku vs. Amazon Web Services for Startups
---
If we search for a comparison of Heroku or AWS, we’ll see a bunch of articles that juxtapose AWS Elastic Compute Cloud (EC2) with Heroku. But comparing EC2 and Heroku isn’t very logical for several reasons, as we’ll explain shortly.

### AWS Elastic Compute Cloud
Elastic Compute Cloud (EC2) is an Infrastructure-as-a-Service (IaaS) product and is Amazon’s flagship AWS offering. Before we’re able to deploy an application on Elastic Compute Cloud, we have to develop server infrastructure that will suit our application.

But what does that look like? Put simply, we’ll need to manually configure and maintain virtualized servers that run our application. We also add database instances, choose and set up an operating system, and set up a load balancer to spread the load across multiple application servers. On top of that, we must select a CPU and RAM and storage that satisfy our application’s need. We’ll also install backup servers and hook them up to the main servers.

AWS Elastic Compute Cloud provides us only with the building blocks. Our task is to select the best blocks for our application and actively manage them, not only set them up. At RubyGarage, our dedicated DevOps engineer is responsible for provisioning EC2 instances, controlling application deployment, and orchestrating EC2 infrastructure (deciding how these ‘building blocks’ interact with each other).

### Heroku
Now let’s see what Heroku offers. Heroku is a Platform as a Service (PaaS) product based on AWS, and is vastly different from Elastic Compute Cloud. It’s very important to differentiate ‘Infrastructure as a Service’ and ‘Platform as a Service’ solutions as we consider deploying and supporting our application using these two solutions.

Heroku is way simpler to use than AWS Elastic Compute Cloud. Perhaps it’s even too simple. But there’s a good reason for this simplicity. The Heroku platform equips us with a ready runtime environment and application servers. Plus, we benefit from seamless integration with various development instruments, a pre-installed operating system, and redundant servers.

Therefore, with Heroku, we don’t need to think about infrastructure management, unlike with AWS EC2. We only need to choose a subscription plan and change our plan when necessary.

As we can see, Heroku conveniently takes care of the details. Thus, we can throw all our efforts into application development. You only need a web developer – or multiple developers – to create an application and push it to Heroku using Git. All management is done via the Heroku Command Line Interface or in the Heroku Dashboard.

Сomparing AWS Elastic Compute Cloud to Heroku is like comparing a microwave to a toaster. Both devices are used for heating food, but they work differently. Maybe this metaphor isn’t the most apt, but it gets across the general point: We use AWS EC2 and Heroku to reach different goals.

So, to be reasonable, we must mention another AWS product that is a direct competitor to Heroku. This product is called Elastic Beanstalk, and it’s also a Platform as a Service product.

### AWS Elastic Beanstalk
AWS offers Elastic Beanstalk to simplify application deployment.

Similar to Heroku, we deploy applications on AWS Elastic Beanstalk by running commands in a Command Line Interface (provided by AWS) or by using the Management Console. After deployment, Elastic Beanstalk manages infrastructure without our control.

We generally don’t need to set up capacity provisioning, load balancing, or scaling, although we’re still able to get access to the infrastructure, if necessary, and save multiple configuration options for our application. Elastic Beanstalk uses EC2 instances to host your application, so migrating from AWS Beanstalk to EC2 is easy. And that’s great.

### AWS vs. Heroku Features
<table> 
 <tbody> 
  <tr> 
   <td><strong>Service</strong></td> 
   <td><strong>AMAZON WEB SERVICES</strong></td> 
   <td><strong>HEROKU</strong></td> 
  </tr> 
  <tr> 
   <td><p>Offered by</p></td> 
   <td><p>Amazon, hosted on proprietary servers</p></td> 
   <td><p>Salesforce, hosted on Amazon Web Services</p></td> 
  </tr> 
  <tr> 
   <td><p>Pricing</p></td> 
   <td><p>Pay-as-you-go</p></td> 
   <td><p>Pay-as-you-go</p></td> 
  </tr> 
  <tr> 
   <td><p>Main Offerings</p></td> 
   <td><p>Platform as a Service<br><strong>(Elastic Beanstalk)</strong></p><p>Infrastructure as a Service<br><strong>(Elastic Compute Cloud)</strong></p></td> 
   <td><p>Platform as a Service</p></td> 
  </tr> 
  <tr> 
   <td><p>Concept</p></td> 
   <td><p>Ready platform for rapid application deployment<br><strong>(Elastic Beanstalk)</strong></p><p>Infrastructure, which must be set up before deployment and managed afterwards<br><strong>(Elastic Compute Cloud)</strong></p></td> 
   <td><p>Ready platform for rapid application deployment</p></td> 
  </tr> 
  <tr> 
   <td><p>Supported platforms</p></td> 
   <td><p>Runs environments for Ruby, NodeJS, Python, Go, Docker, PHP, and .NET applications</p></td> 
   <td><p>Initially designed to deploy Ruby on Rails applications<br>Runs environments for Python, PHP, Clojure, Go, Java, Scala, and Node.js applications</p></td> 
  </tr> 
  <tr> 
   <td><p>Scaling</p></td> 
   <td><p>Supports automatic scaling for EC2 and Beanstalk based on time and metrics</p><p>Can set up the AutoScale feature before deploying your application</p></td> 
   <td><p>Supports manual scaling with the help of the Scaling slider in Heroku Dashboard or via a Command Line Interface</p></td> 
  </tr> 
  <tr> 
   <td><p>Geographic&nbsp;<br>availability</p></td> 
   <td><p>Throughout the world</p></td> 
   <td><p>US and Europe</p></td> 
  </tr> 
  <tr> 
   <td><p>Main Features</p></td> 
   <td><p><strong>Elastic Beanstalk</strong><br>Capacity Provisioning<br>Load Balancing<br>Auto-Scaling<br>App Health Monitoring</p><p><strong>Elastic Compute Cloud</strong><br>Ready templates for deployment<br>Multiple configurations (CPU, RAM, etc.)</p></td> 
   <td><p>Capacity Provisioning<br>Database Rollback<br>Application Rollback<br>Manual Vertical and Horizontal Scaling<br>App Health Monitoring<br>Full GitHub Integration</p></td> 
  </tr> 
  <tr> 
   <td><p>Architecture</p></td> 
   <td><p><strong>Standard server architecture:</strong></p><p>Web server/load balancer<br>Platform<br>Operating System<br>Application tier<br>Database tier</p></td> 
   <td><p><strong>Standard server architecture:</strong></p><p>Web server/load balancer<br>Platform<br>Operating System<br>Application tier<br>Database tier</p></td> 
  </tr> 
  <tr> 
   <td><p>Built-in Tools for Management and Monitoring</p></td> 
   <td><p>AWS Management Console<br>AWS Command Line Interface (AWS CLI)<br>AWS CloudWatch</p></td> 
   <td><p>Heroku Command Line<br>Heroku Application Metrics<br>Heroku Connect<br>Heroku Status</p></td> 
  </tr> 
  <tr> 
   <td><p>Service Level&nbsp;<br>Agreements</p></td> 
   <td><p>Available for Elastic Compute Cloud</p></td> 
   <td><p>Available for Enterprise projects</p></td> 
  </tr> 
 </tbody> 
</table>

### Conclusion
When choosing between AWS and Heroku, you primarily need to consider the costs. Will it cost less for you to manage infrastructure yourself, or is it cost-effective for you to reply on a ready (but somewhat costly) platform that manages your infrastructure for you?

In summary, you should use AWS Elastic Compute Cloud when:

- You need infrastructure flexibility from the first deployment of your application.
- You can afford a DevOps engineer or several DevOps engineers to manage the infrastructure.
- You’re ready to spend more time deploying new versions of your app.
- Your project demands great computational resources.

And you should use Heroku or AWS Elastic Beanstalk when:

- You need to deploy and test a Minimum Viable Product.
- You need to improve your application quickly after getting feedback from users.
- You can’t afford a DevOps engineer (or engineers).
- Your project doesn’t demand that many computational resources.

If you do choose Amazon Web Services, it’s important to make sure that the company you’re working with has experience managing AWS infrastructure. And if rapid application development is your highest priority, consider Heroku or Beanstalk. Keep in mind that you can always switch between Heroku and AWS EC2 should hosting plans change or your application demands a custom infrastructure. Still, it’s best to start with the right service right away.

- https://www.heroku.com/platform
- https://www.heroku.com/dynos