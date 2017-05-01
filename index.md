email: sam at this domain

[LinkedIn][2]

Sam lives in [El Cerrito][1].

[1]: https://maps.google.com/maps?q=El+Cerrito,+CA&hl=en&sll=37.269174,-119.306607&sspn=12.998261,16.831055&oq=el+ce&hnear=El+Cerrito,+Contra+Costa+County,+California&t=m&z=14
[2]: http://www.linkedin.com/profile/view?id=21062260

##Recent Projects
###Chef automation
* ~40 custom cookbooks for in-house applications
* ~30 wrapper cookbooks to customize official cookbooks
* ~90 server roles
* ~5 Chef environments for development (one per team), one for staging, and one for production. All configuration changes can be tested before going into production.
* ~400 nodes under Chef control
* OpsCode's hosted Chef service
* Berkshelf for cookbook dependancy management
* Chef search (elasticsearch) is used for configure-time service discovery. For instance, database master and slave servers can be taught to automatically discover each other, exchange credentials, and set up firewall rules to communicate with each other.

###Component Readmes
This is an ongoing project to document each part of our system with an operations audience in mind.

I identified a need for an operations handoff document and wrote the first example readme. I coached and gave feedback to other developers as they were writing readmes for their components.

Readmes are the starting point for writing chef recipes, nagios checks, and emergency runbooks. Each readme includes everything you need to run and monitor a single component. They describe customer-facing components, back-end components, and 3rd party software used for internal infrastructure.

Readmes are based on a standard template which includes:

* Availability Requirements
* Business effects - Availability requirements and customer-visible effects.
* Data responsibility. What data is this component responsible for and how do you make backups of it?
* Deployment considerations - special requirements for installation and upgrades
* Service Dependencies - which internal and 3rd party services/components does this component depend on?
* Architecture description - what kind of failures can it tolerate?
* Health check procedures - positive and negative health indicators
* Failover and disaster recovery procedures
* Routine maintenance procedures
* Known Operational Issues and Workarounds

##Languages / Frameworks
* Ruby
	* RVM, rubygems, Bundler
	* Ruby on Rails 3, REST APIs
	* Chef (berkshelf, knife-vsphere)
	* Capistrano
* JavaScript and CoffeeScript
	* Ember.js and SproutCore
	* Google Maps API (older versions)

##Software
* Subversion to Git transition, including introductory training
* MySQL - intermediate tuning, built-in replication
* RabbitMQ
* ZooKeeper
* Redis
* Memcached
* Amazon S3 (key/value store), Route53 (DNS), EC2
* Vagrant (automatic VM creation)
* Jenkins - basic

##Software Development
* Scrum
* introductory tech talks on Ruby and Git
* TDD/BDD with RSpec

##Things I'd like to work on
###Concepts / Architecture / Ideas

* Comprehensive automation.
	* Your infrastructure configuration should be described in a machine readable format and stored in a revision control system
	* You should be able to configure a whole datacenter without manual intervention.
	* If you find it necessary to log in to a system to perform an action, you should open a ticket so that your task can eventually be automated.
* Orchestration - how do you model, automate, and change-manage operational events like software upgrades, architectural changes, datacenter moves, failover events, etc-
* Share-nothing / eventually consistent architectures like Wave Operational Transform, Dynamo/Cassandra/Riak, etc.
* Tools to reinforce good development habits like using Gerrit to make code reviews an automatic part of the develoment process.
* Present common operational tasks through an easily customizable UI like Jenkins so that these tasks are easy to perform in a consistent manner and there is a record of who made a change and when it was made.

###Specific Software

* logstash / kibana / elasticsearch
* http://mesos.apache.org/ Cluster manager. like google borg, but from twitter
* http://airbnb.github.io/chronos/ cron replacement that runs on top of Mesos
* Cassandra or Riak
* Linux containers / BSD jails / Solaris Zones
* Some kind of SQL proxy to support transparent failover to a hot spare

##Other Interests
* coffee (ex-barrista)
* cars, from a technical standpoint (ex-mechanic)
* armchair cognitive science
* woodworking