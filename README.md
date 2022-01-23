<img width="500" src="https://wlsdm.com/wl-opc/docs/docs/assets/brand/wl-opc-with-subtitle.svg">

<b>WL-OPC is the central operation system to manage and monitor Oracle WebLogic Server and FMW products.</b>

<a href="https://wlsdm.com/wl-opc" target="_blank">https://wlsdm.com/wl-opc</a>

# Getting Started 

WL-OPC (WLSDM OPERATION CENTER) is the central Operation and Notification system that enables to manage and monitor Oracle WebLogic Server infrastructures and Oracle Fusion Middleware domains such as Oracle ADF, SOA Suite, Oracle Service Bus (OSB), Business Intelligence (OBIEE), E-Business Suite (EBS)... etc.

### Monitor, Manage, Organize and Bulk Update: Unlimited Oracle WebLogic & Oracle Fusion Middleware Domains

<table>
<tr>
<td style='border:none;'><img alt="WL-OPC" src="https://wlsdm.com/wl-opc/docs/docs/assets/img/menu.png" width="250"></td>
<td style='border:none;'>
<ul>
    <li>Oracle WebLogic FMW Domains Asset Management and Inventory</li>
    <li>Oracle WebLogic AdminServer Monitoring</li>
    <li>Central HEALTH and STATE Monitoring (Servers, Deployments, Data Sources, JMS Resources, FMW Components)</li>
    <li>Consolidated and Central Notification Dashboard (Garbage Collection, JVM Resources, Back-end... etc.)</li>
    <li>Central WLSDM Notification Broadcasting and Notification Rules</li>
    <li>Reporting WebLogic Domain Performance and Availability</li>
    <li>Comparing WebLogic JVM Arguments</li>
    <li>Bulk JVM Argument Manager</li>
    <li>Bulk Data Source Manager</li>
    <li>Bulk Domain Settings Standardizer</li>
</ul>
</td>
</tr>
</table>

# Available Tags

* <code>latest</code>
* <code>v2.0.1-b964</code>

# WL-OPC Architecture

<img width="100%" src="https://wlsdm.com/wl-opc/docs/docs/assets/img/wlopc_installation_best_practice.svg">

# Supported Oracle FMW Products 

* WL-OPC completes below Oracle Fusion Middleware (FMW) products with the best and lightest central monitoring infrastructure
* WL-OPC is the only product that understands multiple Oracle WebLogic FMW domain management and offers the best tools for WebLogic Developers and Administrators
* Supports Oracle 11g, 12c and 14c compatible versions

<br>

<table class="table-striped table-bordered table-condensed" style="margin-left: 20px;">
    <tr>
        <td>&nbsp;Oracle ADF</td>
    </tr>
    <tr>
        <td>&nbsp;Oracle SOA Suite</td>
    </tr>
    <tr>
        <td>&nbsp;Oracle BPM Suite</td>
    </tr>
    <tr>
        <td>&nbsp;Oracle Service Bus (OSB)</td>
    </tr>
    <tr>
        <td>&nbsp;Oracle Business Intelligence (OBIEE, BI Publisher)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</td>
    </tr>
    <tr>
        <td>&nbsp;Oracle Coherence</td>
    </tr>
    <tr>
        <td>&nbsp;Oracle Data Integrator (ODI)</td>
    </tr>
    <tr>
        <td>&nbsp;Oracle Data Service Integrator</td>
    </tr>
    <tr>
        <td>&nbsp;Oracle Forms and Reports</td>
    </tr>
    <tr>
        <td>&nbsp;Oracle Identity Management (IDM)</td>
    </tr>
    <tr>
        <td>&nbsp;Oracle Access Manager (OAM)</td>
    </tr>
    <tr>
        <td>&nbsp;Oracle Virtual Directory (OVD)</td>
    </tr>
    <tr>
        <td>&nbsp;Oracle Unified Directory</td>
    </tr>
    <tr>
        <td>&nbsp;Oracle Internet Directory (OID)</td>
    </tr>
    <tr>
        <td>&nbsp;Oracle WebCenter</td>
    </tr>
    <tr>
        <td>&nbsp;Oracle HTTP Server (OHS)</td>
    </tr>
    <tr>
        <td>&nbsp;Oracle Traffic Director (OTD)</td>
    </tr>
    <tr>
        <td>&nbsp;Oracle Primavera P6</td>
    </tr>
    <tr>
        <td>&nbsp;Oracle Utilities Application Framework (OUAF)</td>
    </tr>
    <tr>
        <td>&nbsp;Oracle Customer Care and Billing (CC&B)</td>
    </tr>
    <tr>
        <td>&nbsp;Oracle Utilities Meter Data Management (MDM)</td>
    </tr>
    <tr>
        <td>&nbsp;Oracle Utilities Customer to Meter (C2M)</td>
    </tr>
</table>

# Installation Using Docker Image

## Easy and Quick Installation Using Docker Image

1. Download latest  <b>JDK 11.x.x Linux x64 Compressed Archive file</b> from oracle.com (i.e. jdk-11.0.13_linux-x64_bin.tar.gz)
<p><a href="https://www.oracle.com/java/technologies/javase/jdk11-archive-downloads.html" target="_blank"><code><b>Download: </b>https://www.oracle.com/java/technologies/javase/jdk11-archive-downloads.html</code></a></p>

2. Download  <b>Dockerfile</b> file from wlsdm.com
<p><a href="https://wlsdm.com/download_manager?FILE_NAME=Dockerfile" target="_blank"><code><b>Download: </b>https://wlsdm.com/download_manager?FILE_NAME=Dockerfile</code></a></p>

3. Download  buildRunDockerImage.sh file from wlsdm.com
<p><a href="https://wlsdm.com/download_manager?FILE_NAME=buildRunDockerImage.sh" target="_blank"><code><b>Download: </b>https://wlsdm.com/download_manager?FILE_NAME=buildRunDockerImage.sh</code></a></p>

4. Execute  <b>buildRunDockerImage.sh</b> script to build & run WL-OPC docker container image
<br><br>

### Summary of Commands: Help, Build and Run

<pre>
<b>Help :</b>  ./buildRunDockerImage.sh -h<br>
<b>Build :</b> ./buildRunDockerImage.sh -b<br>
<b>Run :</b>   ./buildRunDockerImage.sh -i 10.0.0.2 -r<br>
</pre>

<br>

## 4.1. buildRunDockerImage.sh -b

<pre>
<code>$./buildRunDockerImage.sh -b                    

======================
# BUILDING THE IMAGE #
======================

    [INFO]  Building image named 'volthread/wlopc:v2.0.1-b955' ...
    [INFO]  Building image using '/Users/admineer/u01/opc.wlsdm/docker/docker-rt/Dockerfile' ...
    [INFO]  Building WL-OPC with line: 
            docker build --force-rm=true --no-cache=true -t volthread/wlopc:v2.0.1-b955 -f /Users/admineer/u01/opc.wlsdm/docker/docker-rt/Dockerfile .

[+] Building 14.4s (11/11) FINISHED                                                                                                                                                                                                                          
    => [internal] load build definition from Dockerfile                                                                                                                                                                                                    0.0s
    => => transferring dockerfile: 37B                                                                                                                                                                                                                     0.0s
    => [internal] load .dockerignore                                                                                                                                                                                                                       0.0s
    => => transferring context: 2B                                                                                                                                                                                                                         0.0s
    => [internal] load metadata for docker.io/library/centos:8                                                                                                                                                                                             1.7s
    => [auth] library/centos:pull token for registry-1.docker.io                                                                                                                                                                                           0.0s
    => CACHED [1/5] FROM docker.io/library/centos:8@sha256:a27fd8080b517143cbbbab9dfb7c8571c40d67d534bbdee55bd6c473f432b177                                                                                                                                0.0s
    => [internal] load build context                                                                                                                                                                                                                       0.0s
    => => transferring context: 562B                                                                                                                                                                                                                       0.0s
    => [2/5] RUN mkdir /u01 &&     useradd -b /u01 -d /u01/opc -m -s /bin/bash opc &&     mkdir -p /u01/opc/setups &&     mkdir -p /u01/opc/jdk/latest &&     chmod -R 775 /u01/opc                                                                        0.7s
    => [3/5] WORKDIR /u01/opc                                                                                                                                                                                                                              0.0s
    => [4/5] COPY jdk-11.0.13_linux-x64_bin.tar.gz wl-opc.zip /u01/opc/setups/                                                                                                                                                                      3.3s
    => [5/5] RUN tar --extract --file /u01/opc/setups/jdk-11.0.13_linux-x64_bin.tar.gz --directory /u01/opc/jdk/latest --strip-components 1 &&     cd /u01/opc ; /u01/opc/jdk/latest/bin/jar -xvf /u01/opc/setups/wl-opc.v2.0.1.zip &&     rm -rf /u01/op  6.0s
    => exporting to image                                                                                                                                                                                                                                  2.5s
    => => exporting layers                                                                                                                                                                                                                                 2.5s
    => => writing image sha256:6135c58a9da3483e75d11f6bb5c56a1c2f7a2a15ff6734b112ab8601d88aeba5                                                                                                                                                            0.0s 
    => => naming to docker.io/volthread/wlopc:v2.0.1-b955                                                                                                                                                                                                  0.0s 
                                                                                                                                                                                                                                                                
Use 'docker scan' to run Snyk tests against images to find vulnerabilities and learn how to fix them                                                                                                                                                         
======================
#  TAGING THE IMAGE  #
======================

    [INFO]  Taging image 'volthread/wlopc:v2.0.1-b955' as latest
    [INFO]  WL-OPC Docker image for version v2.0.1-b955 is ready to be used
    [INFO]  Docker Image Name --> volthread/wlopc:v2.0.1-b955
    [INFO]  Docker Image Name --> volthread/wlopc:latest
    [INFO]  Build completed in 15 seconds
</code>
</pre>

<br>

## 4.2. buildRunDockerImage.sh -i 10.0.0.2 -r

<pre>
$./buildRunDockerImage.sh -i 10.0.0.2 -r

[INFO]  IP address of Docker host which docker process is running: 10.0.0.2


[INFO]  !!! WLOPC docker persistence volume is missing !!!
[INFO]  Creating docker persistence volume named: WLOPC

[INFO]  Runing WL-OPC docker container image with line: 
docker container run --name=wlopc --hostname=opcprodsrv1 --add-host=opcprodsrv1:10.0.0.2 --net=bridge -d -p 8080:8080 -p 9090:9090 -v WLOPC:/u01/opc/wl-opc/bin/WLOPC volthread/wlopc:latest

ce9a0fa4f76dbfb59687f7169b8f106b1065b74645b905667ad4a4d346eaf293

[INFO]  WL-OPC Docker container for version v2.0.1-b989 is runing and accepting requests! 

[INFO]  WL-OPC Docker container process: 
ce9a0fa4f76d   volthread/wlopc:latest         "/u01/opc/wl-opc/bin…"   1 second ago   Up Less than a second   0.0.0.0:8080->8080/tcp, 0.0.0.0:9090->9090/tcp   wlopc
</pre>
<br>

5. That's all! Access WL-OPC web console  http(s)://$wlopc-server-ip:$port/opc

6. Login to the WL-OPC Console then complete the configuration wizard for once (Default Credentials:  <code>admin/wl-opc</code>)

# Easy Build & Run With buildRunDockerImage.sh

 <b>buildRunDockerImage.sh</b> script is used for "build & run" WL-OPC Docker image for on-premise production server installations. This script facilitates build&run WL-OPC Docker image  for production environment server which does not have internet access. Before proceeding, make sure you meet the system requirements and prerequisites.


<pre>
# https://wlsdm.com | https://www.volthread.com
# Copyright (c) 2017, 2022, Volthread and/or its affiliates
# Licensed under WL-OPC End-User License Agreement (EULA)
# This End-User License Agreement ("EULA") is a legal agreement between you (either an individual or a single legal entity) WL-OPC (WLSDM Operation Center), which covers your use of WL-OPC and related software components
# EULA is available at https://wlsdm.com/wl-opc/docs/lic/wl-opc-license.txt

# ******************************************************************************
#
# Usage: sh buildDockerImage.sh [-c]
# Builds Docker image or runs Docker container for WL-OPC (WLSDM Operation Center)
# Parameters: Docker Build & Container Run Parameters are available below
# For advanced settings and usage edit parameter values then pass arguments
#
# ******************************************************************************

"Build & Run" Docker Image for WL-OPC (WLSDM Operation Center)

Build Usage : ./buildRunDockerImage.sh [ -g | -d ] [ -c ] [ -b ]
Run Usage   : ./buildRunDockerImage.sh [ -v ] [ -n $WLOPC_DOCKER_NW_MODE ] [ -i $WLOPC_DOCKER_HOST_IP ] [ -r ]

Parameters & Options: Select build or run option only; -b or -r

   * Select BUILD (-b) or RUN (-r) option only. Build and Run options are not allowed to be executed at the same time. -b or -r
  ** Parameters and arguments must be passed in order and positional


  ----------
  -b (build)
  ----------
  -c : enables docker image layer cache during the build (default is --no-cache=true)
  -b : builds docker image with the default Dockerfile

  Example Build Usage                     : sh buildRunDockerImage.sh -b
  Example Build Usage with Enabling Cache : sh buildRunDockerImage.sh -c -b

  --------  
  -r (run)
  --------
  -i : IP address of docker host (server/machine)  
  -v : docker persistence volume name or full path of WL-OPC runtime folder on docker host machine. Default volume name is WLOPC and it is created automatically if does not exist
  -n : docker network mode (default is host)
  -r : run WL-OPC docker container

  Example Run Usage                   : sh buildRunDockerImage.sh -i 10.0.0.2 -r
  Example Run Usage with Volume       : sh buildRunDockerImage.sh -i 10.0.0.2 -v WLOPC-PROD-DATA -r
  Example Run Usage with Local Volume : sh buildRunDockerImage.sh -i 10.0.0.2 -v /data/opc/WLOPC -r
  Example Run Usage with Network Mode : sh buildRunDockerImage.sh -i 10.0.0.2 -n bridge -r

  ---------  
  -h (help)
  ---------

  -h : prints usage of buildRunDockerImage.sh
</pre>


# Step by Step Installation Guide for WL-OPC Docker Image

Using Docker Image Installation guide for production environment is available.

### Go to Installation Using Docker Image Guide

<a href="https://wlsdm.com/wl-opc/docs/readme##step-by-step-installation-using-docker-image" target="_blank">https://wlsdm.com/wl-opc/docs/readme##step-by-step-installation-using-docker-image</a>

# Quick References

* <b>Documentation ReadMe > </b> <a href="https://wlsdm.com/wl-opc/docs/readme" target="_blank">https://wlsdm.com/wl-opc/docs/readme</a><br>
* <b>Documentation Help > </b> <a href="https://wlsdm.com/wl-opc/docs/help" target="_blank">https://wlsdm.com/wl-opc/docs/help</a><br>
* <b>Community Help > </b> <a href="https://community.wlsdm.com" target="_blank">https://community.wlsdm.com</a><br>
* <b>Medium Blog > </b> <a href="https://blog.wlsdm.com" target="_blank">WLSDM Blog | https://blog.wlsdm.com</a><br><br>
* <b>Customer Support > </b> <a href="https://support.volthread.com" target="_blank">Volthread Support System (VSS) | https://support.volthread.com</a><br>
* <b>Maintained By > </b> <a href="https://www.volthread.com" target="_blank">Volthread Technology | https://www.volthread.com</a><br>

# License

The license agreement (EULA) can be found on <a href="https://wlsdm.com/wl-opc/docs/lic/wl-opc-license.txt" target="_blank">wlopc-license.txt</a>  page which is located in the "lic" folder

<b>Copyright (c) 2022 | Volthread and/or its affiliates.</b>
