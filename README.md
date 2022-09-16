# C3G ARC Group


The c3g advance research computing (ARC) group support the center research objectives by making available computing resources they need.

We want to provide the resources as much as possible is a digested form like PaaS or SaaS, as opposed to the RAW IaaS form.    


## Our resources  

Our hardware resources are mainly:

* [The SD4H secure cloud](https://www.sd4health.ca/)
* [Juno (the old secure cloud)](https://esc.calculquebec.ca/auth/login/?next=/)
* [The Alliance Systems (mainly HPC, but also cloud tape services)](https://docs.alliancecan.ca/wiki/Technical_documentation)

We also have human resources to support us.
First, we can rely to some extent on the Genome Center (GC) IT group, especially when it comes to make sure that our systems are well connected to the GC HPC and storage systems or to other hardware related to the GC sequencing mission, but they are not supporting the hardware resources listed above. Our main service provider and collaborators are from [Calcul Québec](https://www.calculquebec.ca/) (CQ) and from the [Digital Research Alliance of Canada](https://alliancecan.ca/) (the Alliance). From their point of view, we are a local service provider and we can rely on them to access regional services, provided by CQ and national services, provided by the Alliance. The Alliance is a federation of groups, some like us integrated in to a research group and supporting them directly and other integrated to regional or national service teams. The main way of communication with then is through the [CQ](https://calculquebec.slack.com) and [Alliance](https://alliancecan.slack.com) slack channels.

## The people we serve


We can split the people we help in two groups, an internal one, which mainly comprise C3G staff and their projects and then external user related to the SD4H platform. Our procedure is typically to develop and deploy service for the C3G team and then make that service robust enough so it can be offered more broadly to the SD4H users.

Form the CQ and the Alliance perspective, we are offering local service where they are respectively responsible to offer regional and national service.


## The kind of service we offer

On a more concrete level, we write code and documentation so that infrastructure we have is able to do what the C3G wants to do with it! But, then what does the C3G wants?

First, the Tech/Dev group. Is mainly composed of bioinformatician. They develop benchmark and run the (Genpipes)[https://genpipes.readthedocs.io] analysis pipelines as well as other bioinfo tools. They generate large amount of data and they need to move that data around, they are also hopefully transitioning do databases to track the location and state of their data.

Here is some of the tools we work on for them at the moment:

* [Continuous integration testing](https://jenkins.vhost38.genap.ca/)
* Mugqic [CVMFS](https://cvmfs.readthedocs.io) stack
* [Genpipes in a Container](https://hub.docker.com/r/c3genomics/genpipes/)
* [Magic Castle](https://github.com/ComputeCanada/magic_castle/)
* The access to their platform is secure as well as easy.

Here are some of the things we expect doing for them in the future:

  * Database management so they can track process and data
  * Deploy some kind of [Nexflow Execution engine](https://www.nextflow.io/docs/latest/executor.html)

Note that the TechDev groups work in close collaboration with the Service group that help then run analysis on large project, like the Marathon of Hope (MoH).


The second group we serve is the Data group. One of their project is the [Bento platform](https://github.com/bento-platform). They also work on a [LIMS](https://en.wikipedia.org/wiki/Laboratory_information_management_system), called [freezeman](https://github.com/c3g/freezeman).

The data group develops web front end and back end system to share and manage research data. As such they have front end and back end developer, they also have data architect, which can come handy. For them:

* Make sure they has the right architecture and tooling do develop and deploy their platforms.
* They can easily deploy their services on the SD4H platform in a more general sense.
* The access to their platform is secure as well as easy.



----------------------------------------------------------

I want to be more specific with what we want to do with the data group. Then is another sectonc describe the specific services and what they will do exactly. 





  * Collaborate with the CQ administrator so make sure that the OpenStack configuration is right so to enable our activities. This is the [first requirement document](https://docs.google.com/document/d/1yC_ASp9prl9D2stVEH1ryYWroZMCQ6qo5-kWa0lZxOU/) we have with them.  


* Deploy and maintain an authentication service that will serve as a gatekeeper for as much of our services as possible.
