Your answers to the questions go here.

##level 1:
###In your own words, what is the Agent?

* The Agent is open source monitoring and software that collects your data and sends it to DataDog where you can see and interact with it. It runs on your host and collects data without being intrusive or resource heavy. 

###Tags added
tags: my first tag, env:test, role:db
![screenshot of tags on agent](/tags from Agent config file.png)

###code for custom check 

test.support.random 
```python
 from checks import AgentCheck
import random

class RandomCheck(AgentCheck):
	def check(self, instance):
		num = random.random()
		self.gauge('test.support.random', num)
```

##Level 2:

###What is the difference between a timeboard and a screenboard?
* A timeboard has an automatic layout with all your metrics and graphs time synchronized and can be shared individually. 

* A screenboard is more customizable, and can give you a more flexible look into your system, allows for read-only sharing, and every widget has an individual time window. 
![snapshot of box around above .90](/snapshot of above .90.png)

##Level 3:
link to dashboard:
[dashboard](https://p.datadoghq.com/sb/237636259-745aba0497)
![screen shot of custom agent check](/custom agent check.png)
![screen shot of email for downtime](/email for downtime.png)
![screen shot of email for monitor trigger](/email for monitor trigger.png)







