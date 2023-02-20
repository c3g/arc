# C3G ARC Group


The c3g Advance Research Computing (ARC) group support the center research objectives by making available computing resources they need.

We want to provide the resources as much as possible is a digested form like PaaS or SaaS, as opposed to the RAW IaaS form.    


## Our resources  

Our hardware resources are mainly:

* [The SD4H secure cloud](https://www.sd4health.ca/)
* The elastic secure cloud (esc) also known as the [old secure cloud](https://esc.calculquebec.ca/auth/login/?next=/)
* [The Alliance Systems (mainly HPC, but also cloud tape services)](https://docs.alliancecan.ca/wiki/Technical_documentation)

We also have human resources to support us.

Our main service provider and collaborators are from [Calcul Québec](https://www.calculquebec.ca/) (CQ) and from the [Digital Research Alliance of Canada](https://alliancecan.ca/) (the Alliance). From their point of view, we are a local service provider and we can rely on them to access regional services, provided by CQ and national services, provided by the Alliance. The Alliance is a federation of groups, some like us integrated in to a research lab, while other are integrated to large regional or national service teams. The main way of communication with our regional and national collegues is through slack [CQ](https://calculquebec.slack.com) and [Alliance](https://alliancecan.slack.com).

We can also rely to some extent on the Genome Center (GC) IT group, especially when it comes to make sure that our systems are well connected to the GC HPC and storage systems or to other hardware related to the GC sequencing mission, but the GC IT is not supporting the hardware resources listed above. We can always go the the 7th floor of the GC to meet them, but they also have a [ticketing system](it.genome@mail.mcgill.ca>).

## Our current projects


#### SD4H

Our first project it the SD4H platform itself we want it to be succesfull, to do so we do outreach to potential user and show them how the platform can be leverage. 

#### MoH

The Marathon of Hope is a large sequencing project at the center we want to deliver computing power as well as data management capability to the C3G TechDev so they can process the data efficiently. 

The C3G Data team in also involve in MoH. We help them deploy their bento system on the platform and also make sure they can easily acces and share the data produces by the TechDev team. 

  * Deploye a post gress Database with secure login on the secure cloud.
  * Deploy a [SD4H DRS](https://ga4gh.github.io/data-repository-service-schemas/) with [passport and visas](https://github.com/ga4gh-duri/ga4gh-duri.github.io/blob/master/researcher_ids/ga4gh_passport_v1.md) on the secure cloud
  * Test and deploye the Magic Castle project to run the tumor pair pipeline on the secure cloud. 



#### BQC19

We support the Data team so they can share the BQC19 data.

  * Make sure , in collaboration with CQ, that the [Globus platfom](https://www.globus.org/) is running properly on the secure cloud. 



## Synergy with other C3G groups

First, the Tech/Dev group. Is mainly composed of bioinformatician. They develop benchmark and run the (Genpipes)[https://genpipes.readthedocs.io] analysis pipelines as well as other bio-info tools. They generate large amount of data and they need to move that data around, they are also, transitioning do databases to track the location and state of their data.

Here is some of the tools we support with or for them at the moment:

* [Continuous integration testing](https://jenkins.vhost38.genap.ca/)
* Mugqic [CVMFS](https://cvmfs.readthedocs.io) stack
* [Genpipes in a Container](https://hub.docker.com/r/c3genomics/genpipes/)
* [Magic Castle](https://github.com/ComputeCanada/magic_castle/)


The Data groups goal is too make our data available to the broader comunity. To do so, they develop their own system, the [Bento platform](https://github.com/bento-platform). They also work on a [LIMS](https://en.wikipedia.org/wiki/Laboratory_information_management_system), called [freezeman](https://github.com/c3g/freezeman). They also manage data acces to exeternal group on the Globus Platform. 

The data group develops web front end and back end systems to share and manage research data. As such they have front end and back end developer, they also have data architects, which can comes handy when we want advices or help in these area. We wake sure that:

* They have the right architecture and tooling do develop and deploy their platforms in general, and more specifically on our OpenStack cloud.
* They can identify and onboard users that need access to their platforms with the right idientity management tooling.

This last point about identity is really important and will, in fact be one of the central services that we want to deploy on the SD4H platform.

The TechDev and Data groups works in close collaboration with the Service group. Service help them run analysis and share data on large project. The service team will aslo be the first users of the techdev tools. If we do our work properly with the TechDev and Data teams, Services should be able to use what we have work on witout much problems. They are our first _production_ users.    



### Identity and Autentication


One of the underlying point of all the project we will work on is the identification and autentication of users on the platform. 

We support a [Keycloak](https://www.keycloak.org/) instance to give access to C3G Bento instance and other systems deployed for the C3G.






