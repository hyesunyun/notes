# Survey of Open-Source Cloud Computing Infrastructures
by Hye Sun Yun  
April 2021

## Theme

Survey of open-source cloud computing infrastructures and comparing their customizability, transparency, scalability, and security.

## Importance

Commercial cloud computing services are easy to set up and use,
but there are still limitations.

**LIMITATIONS of Commerical Cloud Computing Services**

1. Lack of privacy and control that some users need
2. Expensive costs for large organizations as they often charge by the hour for CPU time

## Background

In cloud computing services, there are three-levels of offerings: 

1. _**Infrastructure as a Service (IaaS)**_
2. Platform as a Service (Paas)
3. Software as a Service (SaaS)

### Categories of open-source cloud computing infrastructures

1. Hypervisor-based approach
2. Container-based approach

Two common technologies used for the Operating System (OS) interface.

![Hypervisor vs Container](diagram.png)

_from Containers and cloud: From LXC to Docker to Kubernetes. Bernstein, D. (2014)._

## Survey

### Hypervisor-based

1. Eucalyptus - _similar to Amazon EC2_
    - Few options for customization
    - Strong separation between admins and users
2. OpenNebula - _allows significant customizability and transparency for both admins and users_
    - NFS (Network File System) filesystem
3. OpenStack - _very popular open-source cloud infrastructure that supports most if not all hypervisor solutions in the market_
    - Admins can choose parts of architecture they need
    - Scalable up to 1 million physical machines with up to 60 million VMs

### Container-based

1. Docker and Kubernetes - _provides a systematic way to deploy Linux apps inside portable containers and Kubernetes manages the Docker container clusters_
    - Dockerfiles
    - Increased efficiency due to smaller size and can be faster than hypervisor-based cloud
    - Lack isolation

## Conclusion

**Trends & Observations**:

1. Hypervisor-based solutions outnumber container-based solutions
2. No significant/classic research paper on open-source cloud computing since 2012~2014
3. Increasing popularity and adoption of Docker and Kubernetes in industry

**Opinions**:

1. Why hasn't there been any significant novel solution to open-source cloud computing in recent years?
    - Existing open-source solutions seem to be adequate to meet the demands of computing resources as updates to existing infrastructures continue to happen.
    - Majority of cloud computing users do not require open-source solutions and therefore, default to commercial systems.
2. With increasing need for computing resources, more container-based approaches with better security and other novel solutions might be due.

## Papers Surveyed

1. Bernstein, D. _Containers and cloud: From LXC to Docker to Kubernetes_. (2014)
2. Peter Sempolinski and Douglas Thain. _A Comparison and Critique of Eucalyptus, OpenNebula and Nimbus_. (2010)
3. Sefraoui, O., Aissaoui, M., and Eleuldj, M. _OpenStack: Toward an Open-Source Solution for Cloud Computing_. (2012)
    - <u>Supplemental paper</u>: Barkat, A., dos Santos, A. D., and Nguyen Ho, T. T. _Open Stack and Cloud Stack: Open Source Solutions for Building Public and Private Clouds_. (2014)

