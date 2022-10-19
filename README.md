# C3G ARC Group


The c3g Advance Research Computing (ARC) group support the center research objectives by making available computing resources they need.

We want to provide the resources as much as possible is a digested form like PaaS or SaaS, as opposed to the RAW IaaS form.    


## Our resources  

Our hardware resources are mainly:

* [The SD4H secure cloud](https://www.sd4health.ca/)
* [Juno (the old secure cloud)](https://esc.calculquebec.ca/auth/login/?next=/)
* [The Alliance Systems (mainly HPC, but also cloud tape services)](https://docs.alliancecan.ca/wiki/Technical_documentation)

We also have human resources to support us.

Our main service provider and collaborators are from [Calcul Québec](https://www.calculquebec.ca/) (CQ) and from the [Digital Research Alliance of Canada](https://alliancecan.ca/) (the Alliance). From their point of view, we are a local service provider and we can rely on them to access regional services, provided by CQ and national services, provided by the Alliance. The Alliance is a federation of groups, some like us integrated in to a research lab, while other are integrated to large regional or national service teams. The main way of communication with our regional and national collegues is through slack [CQ](https://calculquebec.slack.com) and [Alliance](https://alliancecan.slack.com).


We can also rely to some extent on the Genome Center (GC) IT group, especially when it comes to make sure that our systems are well connected to the GC HPC and storage systems or to other hardware related to the GC sequencing mission, but the GC IT is not supporting the hardware resources listed above. We can always go the the 7th floor of the GC to meet them, but they also have a [ticketing system](it.genome@mail.mcgill.ca>).

## Our projects

We offer support for C3G projects as well as project that comes form outide through the SD4H platfom.    

Our procedure is typically to develop and deploy service for a project that will help other C3G team deliver scientific data and share that data to collaborator or the general public. We want to make sure that what we deliverd software and platform that is well packaged and that the service robust are enough so they can be redeployed for other C3G projects and then be offered more broadly to SD4H projects outside of the C3G.

## The support we offer

On a more concrete level, we write code and documentation so that infrastructure we have is able to do what the C3G wants to do with it! But, then what does the C3G wants?

First, the Tech/Dev group. Is mainly composed of bioinformatician. They develop benchmark and run the (Genpipes)[https://genpipes.readthedocs.io] analysis pipelines as well as other bio-info tools. They generate large amount of data and they need to move that data around, they are also, transitioning do databases to track the location and state of their data.

Here is some of the tools we support with or for them at the moment:

* [Continuous integration testing](https://jenkins.vhost38.genap.ca/)
* Mugqic [CVMFS](https://cvmfs.readthedocs.io) stack
* [Genpipes in a Container](https://hub.docker.com/r/c3genomics/genpipes/)
* [Magic Castle](https://github.com/ComputeCanada/magic_castle/)

Here are some of the things we expect doing for them in the future:

  * Database management so they can track process and data
  * Deploy some kind of [Nexflow Execution engine](https://www.nextflow.io/docs/latest/executor.html)

Note that the TechDev groups work in close collaboration with the Service group that help them run analysis on large project.

The second group we serve is the Data group. One of their projects is the [Bento platform](https://github.com/bento-platform). They also work on a [LIMS](https://en.wikipedia.org/wiki/Laboratory_information_management_system), called [freezeman](https://github.com/c3g/freezeman).

The data group develops web front end and back end system to share and manage research data. As such they have front end and back end developer, they also have data architect, which can could handy if we want advice or help in these area. We wake sure that:

* They have the right architecture and tooling do develop and deploy their platforms in general, and more specifically on our OpenStack cloud.
* They can identify and on board users that need access to their platforms.

This last point about identity is really important and will, in fact be one of the first service that we want to deploy on the SD4H platform.


### Specific services or platform

A [Comanage Registry](https://github.com/Internet2/comanage-registry) instance to give access to Bento clients via the [OIDC protocol](https://openid.net/connect/). This federated authorization platform is pretty flexible. We first want to use it with a local keycloak as the identity provider and the google id of the c3g (computationalgenimics.ca), but would like to also have the [Canadian Access Federation (CAF)](https://www.canarie.ca/identity/caf/), we could also add other provider like google.







----------------------------------------------------------

I want to be more specific with what we want to do with the data group. Then is another section describe the specific services and what they will do for us and/our our users.



  * Collaborate with the CQ administrator so make sure that the OpenStack configuration is right so to enable our activities. This is the [first requirement document](https://docs.google.com/document/d/1yC_ASp9prl9D2stVEH1ryYWroZMCQ6qo5-kWa0lZxOU/) we have with them.  


* Deploy and maintain an authentication service that will serve as a gatekeeper for as much of our services as possible.
