![](docs/demo_guide/images/Apollo_logo.png)


[Apollo](http://apollo.auto) is a high performance, flexible architecture which accelerates the development, testing, and deployment of Autonomous Vehicles.

The DOI for this repository is: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6909534.svg)](https://doi.org/10.5281/zenodo.6909534)

## Table of Contents

1. [Introduction](#introduction)
2. [Prerequisites](#prerequisites)
3. [Individual Versions](#individual-versions)
4. [Architecture](#architecture)
5. [Installation](#installation)
6. [Quick Starts](#quick-starts)
7. [Documents](#documents)

## Introduction

Apollo is loaded with new modules and features but needs to be calibrated and configured perfectly before you take it for a spin. Please review the prerequisites and installation steps in detail to ensure that you are well equipped to build and launch Apollo. You could also check out Apollo's architecture overview for a greater understanding of Apollo's core technology and platforms.

## Prerequisites

* The vehicle equipped with the by-wire system, including but not limited to brake-by-wire, steering-by-wire, throttle-by-wire and shift-by-wire (Apollo is currently tested on Lincoln MKZ)

* A machine with a 8-core processor and 16GB memory minimum 

* NVIDIA Turing GPU is strongly recommended 

* Ubuntu 18.04

* NVIDIA driver version 440.33.01 and above ([Web link](https://www.nvidia.com/Download/index.aspx?lang=en-us))

* Docker-CE version 19.03 and above ([Official doc](https://docs.docker.com/engine/install/ubuntu/))

* NVIDIA Container Toolkit ([Official doc](https://github.com/NVIDIA/nvidia-docker))

**Please note**, it is recommended that you install the versions of Apollo in the following order: **1.0 -> whichever version you would like to test out**. The reason behind this recommendation is that you need to confirm whether individual hardware components and modules are functioning correctly, and clear various version test cases before progressing to a higher and more capable version for your safety and the safety of those around you.

## Individual Versions:

The following diagram highlights the scope and features of each Apollo release:

![](docs/demo_guide/images/Apollo_Roadmap_6_0.png)

[**Apollo 1.0:**](docs/quickstart/apollo_1_0_hardware_system_installation_guide.md)

Apollo 1.0, also referred to as the Automatic GPS Waypoint Following, works in an enclosed venue such as a test track or parking lot. This installation is necessary to ensure that Apollo works perfectly with your vehicle. The diagram below lists the various modules in Apollo 1.0.

![](docs/demo_guide/images/Apollo_1.png)

[**Apollo 1.5:**](docs/quickstart/apollo_1_5_hardware_system_installation_guide.md)

Apollo 1.5 is meant for fixed lane cruising. With the addition of LiDAR, vehicles with this version now have better perception of its surroundings and can better map its current position and plan its trajectory for safer maneuvering on its lane. Please note, the modules highlighted in Yellow are additions or upgrades for version 1.5.

![](docs/demo_guide/images/Apollo_1_5.png)

[**Apollo 2.0:**](docs/quickstart/apollo_2_0_hardware_system_installation_guide_v1.md#key-hardware-components)

Apollo 2.0 supports vehicles autonomously driving on simple urban roads. Vehicles are able to cruise on roads safely, avoid collisions with obstacles, stop at traffic lights, and change lanes if needed to reach their destination.  Please note, the modules highlighted in Red are additions or upgrades for version 2.0.

![](docs/demo_guide/images/Apollo_2.png)

[**Apollo 2.5:**](docs/quickstart/apollo_2_5_hardware_system_installation_guide_v1.md)

Apollo 2.5 allows the vehicle to autonomously run on geo-fenced highways with a camera for obstacle detection. Vehicles are able to maintain lane control, cruise and avoid collisions with vehicles ahead of them.

```
Please note, if you need to test Apollo 2.5; for safety purposes, please seek the help of the
Apollo Engineering team. Your safety is our #1 priority,
and we want to ensure Apollo 2.5 was integrated correctly with your vehicle before you hit the road.
```

![](docs/demo_guide/images/Apollo_2_5.png)

[**Apollo 3.0:**](docs/quickstart/apollo_3_0_quick_start.md)

Apollo 3.0's primary focus is to provide a platform for developers to build upon in a closed venue low-speed environment. Vehicles are able to maintain lane control, cruise and avoid collisions with vehicles ahead of them.

![](docs/demo_guide/images/Apollo_3.0_diagram.png)

[**Apollo 3.5:**](docs/quickstart/apollo_3_5_quick_start.md)

Apollo 3.5 is capable of navigating through complex driving scenarios such as residential and downtown areas. The car now has 360-degree visibility, along with upgraded perception algorithms to handle the changing conditions of urban roads, making the car more secure and aware. Scenario-based planning can navigate through complex scenarios, including unprotected turns and narrow streets often found in residential areas and roads with stop signs.

![](docs/demo_guide/images/Apollo_3_5_Architecture.png)

[**Apollo 5.0:**](docs/quickstart/apollo_3_5_quick_start.md)

Apollo 5.0 is an effort to support volume production for Geo-Fenced Autonomous Driving.
The car now has 360-degree visibility, along with upgraded perception deep learning model to handle the changing conditions of complex road scenarios, making the car more secure and aware. Scenario-based planning has been enhanced to support additional scenarios like pull over and crossing bare intersections.

![](docs/demo_guide/images/Apollo_5_0_diagram1.png)

[**Apollo 5.5:**](docs/quickstart/apollo_5_5_quick_start.md)

Apollo 5.5 enhances the complex urban road autonomous driving capabilities of previous Apollo releases, by introducing curb-to-curb driving support. With this new addition, Apollo is now a leap closer to fully autonomous urban road driving. The car has complete 360-degree visibility, along with upgraded perception deep learning model and a brand new prediction model to handle the changing conditions of complex road and junction scenarios, making the car more secure and aware. 

![](docs/demo_guide/images/Apollo_5_5_Architecture.png)

[**Apollo 6.0:**](docs/quickstart/apollo_6_0_quick_start.md)

Apollo 6.0 incorporates new deep learning models to enhance the capabilities for certain Apollo modules. This version works seamlessly with new additions of data pipeline services to better serve Apollo developers. Apollo 6.0 is also the first version to integrate certain features as a demonstration of our continuous exploration and experimentation efforts towards driverless technology.

![](docs/demo_guide/images/Apollo_6_0.png)

## Architecture

* **Hardware/ Vehicle Overview**

![](docs/demo_guide/images/Hardware_overview_3_5.png)

* **Hardware Connection Overview**

![](docs/demo_guide/images/Hardware_connection_3_5_1.png)

* **Software Overview**

![](docs/demo_guide/images/Apollo_3_5_software_architecture.png)

## Installation

* [Hardware installation guide](docs/quickstart/apollo_3_5_hardware_system_installation_guide.md)
* [Software installation guide](docs/quickstart/apollo_software_installation_guide.md) - **This step is required**
* [Launch and run Apollo](docs/howto/how_to_launch_and_run_apollo.md)

Congratulations! You have successfully built out Apollo without Hardware. If you do have a vehicle and hardware setup for a particular version, please pick the Quickstart guide most relevant to your setup:

## Quick Starts:

* [Apollo 6.0 QuickStart Guide](docs/quickstart/apollo_6_0_quick_start.md)

* [Apollo 5.5 QuickStart Guide](docs/quickstart/apollo_5_5_quick_start.md)

* [Apollo 5.0 QuickStart Guide](docs/quickstart/apollo_5_0_quick_start.md)

* [Apollo 3.5 QuickStart Guide](docs/quickstart/apollo_3_5_quick_start.md)

* [Apollo 3.0 QuickStart Guide](docs/quickstart/apollo_3_0_quick_start.md)

* [Apollo 2.5 QuickStart Guide](docs/quickstart/apollo_2_5_quick_start.md)

* [Apollo 2.0 QuickStart Guide](docs/quickstart/apollo_2_0_quick_start.md)

* [Apollo 1.5 QuickStart Guide](docs/quickstart/apollo_1_5_quick_start.md)

* [Apollo 1.0 QuickStart Guide](docs/quickstart/apollo_1_0_quick_start.md)

## Documents

* [Technical Tutorials](docs/technical_tutorial/README.md): Everything you need to know about Apollo. Written as individual versions with links to every document related to that version.

* [How-To Guides](docs/howto/README.md): Brief technical solutions to common problems that developers face during the installation and use of the Apollo platform

* [Specs](docs/specs/README.md): A Deep dive into Apollo's Hardware and Software specifications (only recommended for expert level developers that have successfully installed and launched Apollo)

* [FAQs](docs/FAQs/README.md)

## Questions

You are welcome to submit questions and bug reports as [GitHub Issues](https://github.com/ApolloAuto/apollo/issues).

## Copyright and License

Apollo is provided under the [Apache-2.0 license](https://github.com/ApolloAuto/apollo/blob/master/LICENSE).

## Disclaimer

Apollo open source platform only has the source code for models, algorithms and processes, which will be integrated with cybersecurity defense strategy in the deployment for commercialization and productization.

Please refer to the Disclaimer of Apollo in [Apollo's official website](http://apollo.auto/docs/disclaimer.html).

## Connect with us
* [Have suggestions for our GitHub page?](https://github.com/ApolloAuto/apollo/issues)
* [Twitter](https://twitter.com/apolloplatform)
* [YouTube](https://www.youtube.com/channel/UC8wR_NX_NShUTSSqIaEUY9Q)
* [Blog](https://www.medium.com/apollo-auto)
* [Newsletter](http://eepurl.com/c-mLSz)
* Interested in our turnKey solutions or partnering with us Mail us at: apollopartner@baidu.com
