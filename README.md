# Nebula docs

## Main website available [here](https://nebula-orchestrator.github.io/), refer to the [documentation](http://nebula.readthedocs.io/en/latest/) for more details about how to install & use.

Readthedocs build badge: ![Build Status](https://readthedocs.org/projects/nebula/badge/)


Nebula is a open source distributed Docker orchestrator designed for massive scales (tens of thousands of servers/worker devices), unlike Mesos/Swarm/Kubernetes it has the ability to have workers distributed on high latency connections (such as the internet) yet have the pods(containers) be managed centrally with changes taking affect (almost) immediately, this makes Nebula ideal for managing a vast cluster of servers\devices across the globe, some example use cases are:

* IoT devices
* appliances\virtual appliances located at clients data centers 
* edge computing
* POS systems

Ever wandered how your going to push an update to that smart fridge your company is working on as it's thousands of devices around the globe?
wish you could have the assurance that your service will always use the latest code\envvars\etc in all of it's edge locations?
want the ability to stop\start a globally distributed service with a single command?

Nebula was designed from the ground up to answer all of this needs and much more, refer to the [documentation](http://nebula.readthedocs.io/en/latest/) if your interested in seeing on how to use it.

This repo is the documentation of Nebula container orchestrator, it uses MKDocs to build the readthedocs hosted documentation.
