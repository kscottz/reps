
Ardent Apalone (December 2017 - December 2018)
----------------------------------------------

+----------------------------------------------------------------------------------------+
| > Required support                                                                     |
+---------------------+---------------------+----------------------+---------------------+
| Architecture        | Ubuntu Xenial       | > MacOS Sierra       | > Windows 10        |
|                     | (16.04)             | > (10.12)            | > (VS2015)          |
+=====================+=====================+======================+=====================+
| > amd64             | > X                 | > X                  | > X                 |
+---------------------+---------------------+----------------------+---------------------+
| > arm64             | > X                 |                      |                     |
+---------------------+---------------------+----------------------+---------------------+

Minimum language requirements:

- C11[^2]
- C++14
- Python 3.5

Dependency Requirements:

+----------------+----------------+----------------+----------------+
| Package        | Ubuntu Xenial  | > MacOS\*\*    | > Windows      |
|                |                |                | > 10\*\*       |
+================+================+================+================+
| CMake          | > 3.5.1        | > 3.11.0       | > 3.10.2       |
+----------------+----------------+----------------+----------------+
| EmPY           | > 3.3.2        | > 3.6.5        | > 3.3.2        |
+----------------+----------------+----------------+----------------+
| Ogre           | > 1.10\*       | > 1.10\*       | > 1.10\*       |
+----------------+----------------+----------------+----------------+
| OpenCV         | > 2.4.9        | > 3.4.1        | > 2.4.13.2\*   |
+----------------+----------------+----------------+----------------+
| Poco           | > 1.7.7\*      | > 1.7.7\*      | > 1.7.7\*      |
+----------------+----------------+----------------+----------------+
| Python         | > 3.5.1        | > 3.6.5        | > 3.6.4        |
+----------------+----------------+----------------+----------------+
| Qt             | > 5.5.1        | > 5.10.0       | > 5.10.0       |
+----------------+----------------+----------------+----------------+
| > **Linux only (used for turtlebot demo)**                        |
+----------------+----------------+----------------+----------------+
| PCL            | > 1.7.2        | > N/A          | > N/A          |
+----------------+----------------+----------------+----------------+

\" \* \" means that this is not the upstream version (available on the
official Operating System repositories) but a package distributed by
OSRF or the community (package built and distributed on custom
repositories).

\" \*\* \" Rolling distributions will see multiple version changes of
these dependencies during their lifetime.

This document only captures the version at the first release of a ROS
distribution and will not be updated as the dependencies move forward.
These versions are thus a low watermark.

Package manager use for dependencies:

- Ubuntu Xenial: apt
- MacOS: Homebrew, pip
- Windows: Chocolatey, pip

Build System Support:

- ament_cmake
- cmake
- setuptools

Middleware Implementation Support:

- eProsima Fast-RTPS
- RTI Connext
- ADLINK OpenSplice

Bouncy Bolson (June 2018 - June 2019)
-------------------------------------

Targeted platforms:

+--------------+-----------------------------------------------------------+---------------+
|              | > Required Support                                        | > Recommended |
|              |                                                           | > Support     |
+--------------+--------------+--------------+--------------+--------------+---------------+
| Architecture | Ubuntu       | > MacOS      | > Windows 10 | Ubuntu       | Debian        |
|              | Bionic       | > Sierra     | > (VS2017)   | Xenial       | Stretch (9)   |
|              | (18.04)      | > (10.12)    |              | (16.04)      | \[s\]         |
|              |              |              |              | \[s\]        |               |
+==============+==============+==============+==============+==============+===============+
| > amd64      | > X          | > X          | > X          | > X \[s\]    | > X \[s\]     |
+--------------+--------------+--------------+--------------+--------------+---------------+
| > arm64      | > X          |              |              | > X \[s\]    | > X \[s\]     |
+--------------+--------------+--------------+--------------+--------------+---------------+

\" \[s\] \" Compilation from source, the ROS buildfarm will not produce
any binary packages for these platforms.

Minimum language requirements:

- C11[^3]
- C++14
- Python 3.5

Dependency Requirements:

+-------------+-------------------------------------------------------+-------------+
|             | > Required Support                                    | Recommended |
|             |                                                       | Support     |
+-------------+-------------+-------------+-------------+-------------+-------------+
| Package     | Ubuntu      | > MacOS\*\* | > Windows   | Ubuntu      | Debian      |
|             | Bionic      |             | > 10\*\*    | Xenial      | Stretch     |
|             |             |             |             | \[s\]       | \[s\]       |
+=============+=============+=============+=============+=============+=============+
| CMake       | > 3.10.2    | > 3.11.0    | > 3.10.2    | > 3.5.1     | > 3.7.2     |
+-------------+-------------+-------------+-------------+-------------+-------------+
| EmPY        | > 3.3.2     | > 3.6.5     | > 3.3.2     | > 3.3.2     | > 3.3.2     |
+-------------+-------------+-------------+-------------+-------------+-------------+
| Ogre        | > 1.10\*    | > 1.10\*    | > 1.10\*    | > 1.10\*    | > 1.10\*    |
+-------------+-------------+-------------+-------------+-------------+-------------+
| OpenCV      | > 3.2.0     | > 3.4.1     | > 3.4.1\*   | > 2.4.9     | > 3.2\*     |
+-------------+-------------+-------------+-------------+-------------+-------------+
| Poco        | > 1.8.0     | > 1.9.0     | > 1.8.0\*   | > 1.8.0\*   | > 1.8.0\*   |
+-------------+-------------+-------------+-------------+-------------+-------------+
| Python      | > 3.6.5     | > 3.6.5     | > 3.6.5     | > 3.5.1     | > 3.5.3     |
+-------------+-------------+-------------+-------------+-------------+-------------+
| Qt          | > 5.9.5     | > 5.10.0    | > 5.10.0    | > 5.5.1     | > 5.7.1     |
+-------------+-------------+-------------+-------------+-------------+-------------+
| > **Linux only (used for turtlebot demo)**                                        |
+-------------+-------------+-------------+-------------+-------------+-------------+
| PCL         | > 1.8.1     | > N/A       | > N/A       | > 1.7.2     | > 1.8.0     |
+-------------+-------------+-------------+-------------+-------------+-------------+

\" \* \" means that this is not the upstream version (available on the
official Operating System repositories) but a package distributed by
OSRF or the community (package built and distributed on custom
repositories).

\" \*\* \" Rolling distributions will see multiple version changes of
these dependencies during their lifetime.

\" \[s\] \" Compilation from source, the ROS buildfarm will not produce
any binary packages for these platforms.

This document only captures the version at the first release of a ROS
distribution and will not be updated as the dependencies move forward.
These versions are thus a low watermark.

Package manager use for dependencies:

- Ubuntu Bionic: apt
- MacOS: Homebrew, pip
- Windows: Chocolatey, pip
- Ubuntu Xenial, Debian Stretch: apt

Build System Support:

- ament_cmake
- cmake
- setuptools

Middleware Implementation Support:

- eProsima Fast-RTPS
- RTI Connext
- ADLINK OpenSplice

Crystal Clemmys (December 2018 - December 2019)
-----------------------------------------------

Targeted platforms:

+--------------+-------------------+--------------+--------------+------------+----------+
| Architecture | Ubuntu Bionic     | > MacOS      | > Windows 10 | Ubuntu     | Debian   |
|              | (18.04)           | > Sierra     | > (VS2017)   | Xenial     | Stretch  |
|              |                   | > (10.12)    |              | (16.04)    | (9)      |
+==============+===================+==============+==============+============+==========+
| > amd64      | > Tier 1          | > Tier 1     | > Tier 1     | > Tier 2   | > Tier 3 |
|              | > \[d\]\[a\]\[s\] | > \[a\]\[s\] | > \[a\]\[s\] | > \[s\]    | > \[s\]  |
+--------------+-------------------+--------------+--------------+------------+----------+
| > arm64      | > Tier 1          |              |              | > Tier 2   | > Tier 3 |
|              | > \[d\]\[a\]\[s\] |              |              | > \[s\]    | > \[s\]  |
+--------------+-------------------+--------------+--------------+------------+----------+

The following indicators show what delivery mechanisms are available for
each platform.

\" \[d\] \" Debian packages will be provided for this platform for
packages submitted to the rosdistro.

\" \[a\] \" Binary releases are provided as a single archive per
platform containing all packages in the Crystal ROS 2 repos file[^4].

\" \[s\] \" Compilation from source.

Middleware Implementation Support:

+---------------------------+------------+---------+---------------+-----------------+
| Middleware Library        | Middleware | Support | Platforms     | Architectures   |
|                           | Provider   | Level   |               |                 |
+===========================+============+=========+===============+=================+
| > rmw_fastrtps_cpp\*      | eProsima   | Tier 1  | All Platforms | All             |
|                           | Fast-RTPS  |         |               | Architectures   |
+---------------------------+------------+---------+---------------+-----------------+
| > rmw_connext_cpp         | RTI        | Tier 1  | All Platforms | All             |
|                           | Connext    |         | except Debian | Architectures   |
|                           |            |         |               | except arm64    |
+---------------------------+------------+---------+---------------+-----------------+
| rmw_opensplice_cpp        | ADLINK     | Tier 2  | All Platforms | All             |
|                           | OpenSplice |         | except Debian | Architectures   |
+---------------------------+------------+---------+---------------+-----------------+
| rmw_fastrtps_dynamic_cpp  | eProsima   | Tier 2  | All Platforms | All             |
|                           | Fast-RTPS  |         |               | Architectures   |
+---------------------------+------------+---------+---------------+-----------------+
| > rmw_connext_dynamic_cpp | RTI        | Tier 2  | All platforms | All             |
|                           | Connext    |         | except Debian | architectures   |
|                           |            |         |               | except arm64    |
+---------------------------+------------+---------+---------------+-----------------+

\" \* \" means default RMW implementation.

Middleware implementation support is dependent upon the platform support
tier. For example a Tier 1 middleware implementation on a Tier 2
platform can only receive Tier 2 support.

Minimum language requirements:

- C11[^5]
- C++14
- Python 3.5

Dependency Requirements:

+-------------+---------------------------------------------------------------+---------------+
|             | > Required Support                                            | Recommended   |
|             |                                                               | Support       |
+-------------+---------------+---------------+---------------+---------------+---------------+
| Package     | Ubuntu Bionic | > MacOS\*\*   | > Windows     | Ubuntu Xenial | Debian        |
|             |               |               | > 10\*\*      | \[s\]         | Stretch \[s\] |
+=============+===============+===============+===============+===============+===============+
| CMake       | > 3.10.2      | > 3.13.3      | > 3.13.3      | > 3.5.1       | > 3.7.2       |
+-------------+---------------+---------------+---------------+---------------+---------------+
| EmPY        | > 3.3.2       | > 3.3.2       | > 3.3.2       | > 3.3.2       | > 3.3.2       |
+-------------+---------------+---------------+---------------+---------------+---------------+
| Gazebo      | > 9.0.0       | > 9.9.0       | > N/A         | > 9.9.0\*     | > 9.8.0\*     |
+-------------+---------------+---------------+---------------+---------------+---------------+
| Ogre        | > 1.10\*                                                                      |
+-------------+---------------+---------------+---------------+---------------+---------------+
| OpenCV      | > 3.2.0       | > 4.0.1       | > 3.4.1\*     | > 2.4.9       | > 3.2\*       |
+-------------+---------------+---------------+---------------+---------------+---------------+
| OpenSSL     | > 1.1.0g      | > 1.0.2q      | > 1.0.2q      | > 1.0.2g      | > 1.1.0j      |
+-------------+---------------+---------------+---------------+---------------+---------------+
| Poco        | > 1.8.0       | > 1.9.0       | > 1.8.0\*     | > 1.8.0\*     | > 1.8.0\*     |
+-------------+---------------+---------------+---------------+---------------+---------------+
| Python      | > 3.6.5       | > 3.7.2       | > 3.7.2       | > 3.5.1       | > 3.5.3       |
+-------------+---------------+---------------+---------------+---------------+---------------+
| Qt          | > 5.9.5       | > 5.12.0      | > 5.10.0      | > 5.5.1       | > 5.7.1       |
+-------------+---------------+---------------+---------------+---------------+---------------+
|                             | > **Linux only**              |                               |
+-------------+---------------+---------------+---------------+---------------+---------------+
| PCL         | > 1.8.1       | > N/A         | > N/A         | > 1.7.2       | > 1.8.0       |
+-------------+---------------+---------------+---------------+---------------+---------------+
| > **RMW DDS Middleware Providers**                                                          |
+-------------+---------------------------------------------------------------+---------------+
| Connext DDS | > 5.3.1                                                       | > N/A         |
+-------------+---------------------------------------------------------------+---------------+
| > Fast-RTPS | > 1.7.0                                                                       |
+-------------+-------------------------------------------------------------------------------+
| OpenSplice  | > 6.9.181127OSS                                                               |
+-------------+-------------------------------------------------------------------------------+

\" \* \" means that this is not the upstream version (available on the
official Operating System repositories) but a package distributed by
OSRF or the community (package built and distributed on custom
repositories).

\" \*\* \" Rolling distributions will see multiple version changes of
these dependencies during their lifetime.

\" \[s\] \" Compilation from source, the ROS buildfarm will not produce
any binary packages for these platforms.

This document only captures the version at the first release of a ROS
distribution and will not be updated as the dependencies move forward.
These versions are thus a low watermark.

Package manager use for dependencies:

- Ubuntu, Debian: apt
- MacOS: Homebrew, pip
- Windows: Chocolatey, pip

Build System Support:

- ament_cmake
- cmake
- setuptools

Dashing Diademata (May 2019 - May 2021)
---------------------------------------

Targeted platforms:

+--------------+-------------------+--------------+--------------+-----------+--------------+
| Architecture | Ubuntu Bionic     | MacOS Sierra | Windows 10   | Debian    | OpenEmbedded |
|              | (18.04)           | (10.12)      | (VS2019)     | Stretch   | / webOS OSE  |
|              |                   |              |              | (9)       |              |
+==============+===================+==============+==============+===========+==============+
| > amd64      | > Tier 1          | > Tier 1     | > Tier 1     | > Tier 3  |              |
|              | > \[d\]\[a\]\[s\] | > \[a\]\[s\] | > \[a\]\[s\] | > \[s\]   |              |
+--------------+-------------------+--------------+--------------+-----------+--------------+
| > arm64      | > Tier 1          |              |              | > Tier 3  | > Tier 3     |
|              | > \[d\]\[a\]\[s\] |              |              | > \[s\]   | > \[s\]      |
+--------------+-------------------+--------------+--------------+-----------+--------------+
| > arm32      | > Tier 2          |              |              | > Tier 3  | > Tier 3     |
|              | > \[a\]\[s\]      |              |              | > \[s\]   | > \[s\]      |
+--------------+-------------------+--------------+--------------+-----------+--------------+

The following indicators show what delivery mechanisms are available for
each platform.

\" \[d\] \" Debian packages will be provided for this platform for
packages submitted to the rosdistro.

\" \[a\] \" Binary releases are provided as a single archive per
platform containing all packages in the Dashing ROS 2 repos file[^6].

\" \[s\] \" Compilation from source.

Middleware Implementation Support:

+--------------------------+------------+---------+--------------+-------------------+
| Middleware Library       | Middleware | Support | Platforms    | Architectures     |
|                          | Provider   | Level   |              |                   |
+==========================+============+=========+==============+===================+
| > rmw_fastrtps_cpp\*     | eProsima   | Tier 1  | All          | All Architectures |
|                          | Fast-RTPS  |         | Platforms    |                   |
+--------------------------+------------+---------+--------------+-------------------+
| > rmw_connext_cpp        | RTI        | Tier 1  | All          | All Architectures |
|                          | Connext    |         | Platforms    | except            |
|                          |            |         | except       | arm64/arm32       |
|                          |            |         | Debian and   |                   |
|                          |            |         | OpenEmbedded |                   |
+--------------------------+------------+---------+--------------+-------------------+
| rmw_cyclonedds_cpp       | Eclipse    | Tier 2  | All          | All Architectures |
|                          | Cyclone    |         | Platforms    |                   |
|                          | DDS        |         |              |                   |
+--------------------------+------------+---------+--------------+-------------------+
| rmw_opensplice_cpp       | ADLink     | Tier 2  | All          | All Architectures |
|                          | OpenSplice |         | Platforms    |                   |
|                          |            |         | except       |                   |
|                          |            |         | Debian and   |                   |
|                          |            |         | OpenEmbedded |                   |
+--------------------------+------------+---------+--------------+-------------------+
| rmw_fastrtps_dynamic_cpp | eProsima   | Tier 2  | All          | All Architectures |
|                          | Fast-RTPS  |         | Platforms    |                   |
+--------------------------+------------+---------+--------------+-------------------+

\" \* \" means default RMW implementation.

Middleware implementation support is dependent upon the platform support
tier. For example a Tier 1 middleware implementation on a Tier 2
platform can only receive Tier 2 support.

Minimum language requirements:

- C++14
- Python 3.5

Dependency Requirements:

+-------------+--------------------------------------------+-----------------------------------+
|             | > Required Support                         | > Recommended Support             |
+-------------+--------------+--------------+--------------+--------------+--------------------+
| Package     | Ubuntu       | > MacOS\*\*  | > Windows    | Debian       | > OpenEmbedded\*\* |
|             | Bionic       |              | > 10\*\*     | Stretch      |                    |
+=============+==============+==============+==============+==============+====================+
| CMake       | > 3.10.2     | > 3.14.4     | > 3.14.4     | > 3.7.2      | 3.16.1 /           |
|             |              |              |              |              | 3.12.2\*\*\*       |
+-------------+--------------+--------------+--------------+--------------+--------------------+
| EmPY        | > 3.3.2                                                                        |
+-------------+--------------+--------------+--------------+--------------+--------------------+
| Gazebo      | > 9.0.0      | > 9.9.0      | > N/A        | > 9.8.0\*    | > N/A              |
+-------------+--------------+--------------+--------------+--------------+--------------------+
| Ogre        | > 1.10\*                                                  | > N/A              |
+-------------+--------------+--------------+--------------+--------------+--------------------+
| OpenCV      | > 3.2.0      | > 4.1.0      | > 3.4.6\*    | > 3.2\*      | > 4.1.0 /          |
|             |              |              |              |              | > 3.2.0\*\*\*      |
+-------------+--------------+--------------+--------------+--------------+--------------------+
| OpenSSL     | > 1.1.0g     | > 1.0.2r     | > 1.0.2r     | > 1.1.0j     | 1.1.1d /           |
|             |              |              |              |              | 1.1.1b\*\*\*       |
+-------------+--------------+--------------+--------------+--------------+--------------------+
| Poco        | > 1.8.0      | > 1.9.0      | > 1.8.0\*    | > 1.8.0\*    | > 1.9.4            |
+-------------+--------------+--------------+--------------+--------------+--------------------+
| Python      | > 3.6.5      | > 3.7.3      | > 3.7.3      | > 3.5.3      | > 3.8.2 /          |
|             |              |              |              |              | > 3.7.5\*\*\*      |
+-------------+--------------+--------------+--------------+--------------+--------------------+
| Qt          | > 5.9.5      | > 5.12.3     | > 5.10.0     | > 5.7.1      | 5.14.1 /           |
|             |              |              |              |              | 5.12.5\*\*\*       |
+-------------+--------------+--------------+--------------+--------------+--------------------+
|                            | > **Linux only**            |                                   |
+-------------+--------------+--------------+--------------+--------------+--------------------+
| PCL         | > 1.8.1      | > N/A        | > N/A        | > 1.8.0      | > 1.8.1            |
+-------------+--------------+--------------+--------------+--------------+--------------------+
| > **RMW DDS Middleware Providers**                                                           |
+-------------+--------------------------------------------+-----------------------------------+
| Connext DDS | > 5.3.1                                    | > N/A                             |
+-------------+--------------------------------------------+-----------------------------------+
| Cyclone DDS | > 0.7.x (Coquette)                                                             |
+-------------+--------------------------------------------------------------------------------+
| > Fast-RTPS | > 1.8.0                                                                        |
+-------------+-----------------------------------------------------------+--------------------+
| OpenSplice  | > 6.9.190403OSS                                           | > N/A              |
+-------------+-----------------------------------------------------------+--------------------+

\" \* \" means that this is not the upstream version (available on the
official Operating System repositories) but a package distributed by
OSRF or the community (package built and distributed on custom
repositories).

\" \*\* \" Rolling distributions will see multiple version changes of
these dependencies during their lifetime. The versions shown for
OpenEmbedded are those provided by the 3.1 Dunfell release series; the
versions provided by the other supported release series are listed here:
<https://github.com/ros/meta-ros/wiki/Package-Version-Differences> .
Note that the OpenEmbedded releases series for which a ROS distro has
support will change during its support time frame, as per the
OpenEmbedded support policy shown here:
<https://github.com/ros/meta-ros/wiki/Policies#openembedded-release-series-support>
. However, it will always be supported by least one stable OpenEmbedded
release series.

\" \*\*\* \" webOS OSE provides this different version.

This document only captures the version at the first release of a ROS
distribution and will not be updated as the dependencies move forward.
These versions are thus a low watermark.

Package manager use for dependencies:

- Ubuntu, Debian: apt
- MacOS: Homebrew, pip
- Windows: Chocolatey, pip
- OpenEmbedded: opkg

Build System Support:

- ament_cmake
- cmake
- setuptools

Eloquent Elusor (November 2019 - November 2020)
-----------------------------------------------

Targeted platforms:

+--------------+-------------------+--------------+--------------+-----------+--------------+
| Architecture | Ubuntu Bionic     | MacOS Mojave | Windows 10   | Debian    | OpenEmbedded |
|              | (18.04)           | (10.14)      | (VS2019)     | Buster    | / webOS OSE  |
|              |                   |              |              | (10)      |              |
+==============+===================+==============+==============+===========+==============+
| > amd64      | > Tier 1          | > Tier 1     | > Tier 1     | > Tier 3  |              |
|              | > \[d\]\[a\]\[s\] | > \[a\]\[s\] | > \[a\]\[s\] | > \[s\]   |              |
+--------------+-------------------+--------------+--------------+-----------+--------------+
| > arm64      | > Tier 1          |              |              | > Tier 3  | > Tier 3     |
|              | > \[d\]\[a\]\[s\] |              |              | > \[s\]   | > \[s\]      |
+--------------+-------------------+--------------+--------------+-----------+--------------+
| > arm32      | > Tier 2          |              |              | > Tier 3  | > Tier 3     |
|              | > \[a\]\[s\]      |              |              | > \[s\]   | > \[s\]      |
+--------------+-------------------+--------------+--------------+-----------+--------------+

The following indicators show what delivery mechanisms are available for
each platform.

\" \[d\] \" Debian packages will be provided for this platform for
packages submitted to the rosdistro.

\" \[a\] \" Binary releases are provided as a single archive per
platform containing all packages in the Eloquent ROS 2 repos file[^7].

\" \[s\] \" Compilation from source.

Middleware Implementation Support:

+--------------------------+------------+---------+--------------+-------------------+
| Middleware Library       | Middleware | Support | Platforms    | Architectures     |
|                          | Provider   | Level   |              |                   |
+==========================+============+=========+==============+===================+
| > rmw_fastrtps_cpp\*     | eProsima   | Tier 1  | All          | All Architectures |
|                          | Fast-RTPS  |         | Platforms    |                   |
+--------------------------+------------+---------+--------------+-------------------+
| > rmw_connext_cpp        | RTI        | Tier 1  | All          | All Architectures |
|                          | Connext    |         | Platforms    | except            |
|                          |            |         | except       | arm64/arm32       |
|                          |            |         | Debian and   |                   |
|                          |            |         | OpenEmbedded |                   |
+--------------------------+------------+---------+--------------+-------------------+
| rmw_cyclonedds_cpp       | Eclipse    | Tier 2  | All          | All Architectures |
|                          | Cyclone    |         | Platforms    |                   |
|                          | DDS        |         |              |                   |
+--------------------------+------------+---------+--------------+-------------------+
| rmw_opensplice_cpp       | ADLINK     | Tier 2  | All          | All Architectures |
|                          | OpenSplice |         | Platforms    |                   |
|                          |            |         | except       |                   |
|                          |            |         | Debian and   |                   |
|                          |            |         | OpenEmbedded |                   |
+--------------------------+------------+---------+--------------+-------------------+
| rmw_fastrtps_dynamic_cpp | eProsima   | Tier 2  | All          | All Architectures |
|                          | Fast-RTPS  |         | Platforms    |                   |
+--------------------------+------------+---------+--------------+-------------------+

\" \* \" means default RMW implementation.

Middleware implementation support is dependent upon the platform support
tier. For example a Tier 1 middleware implementation on a Tier 2
platform can only receive Tier 2 support.

Minimum language requirements:

- C++14
- Python 3.6

Dependency Requirements:

+-------------+--------------------------------------------+-----------------------------------+
|             | > Required Support                         | > Recommended Support             |
+-------------+--------------+--------------+--------------+--------------+--------------------+
| Package     | Ubuntu       | > MacOS\*\*  | > Windows    | Debian       | > OpenEmbedded\*\* |
|             | Bionic       |              | > 10\*\*     | Buster       |                    |
+=============+==============+==============+==============+==============+====================+
| CMake       | > 3.10.2     | > 3.14.4     | > 3.14.4     | > 3.13.4     | 3.16.1 /           |
|             |              |              |              |              | 3.12.2\*\*\*\*     |
+-------------+--------------+--------------+--------------+--------------+--------------------+
| EmPY        | > 3.3.2                                                                        |
+-------------+--------------+--------------+--------------+--------------+--------------------+
| Gazebo      | > 9.0.0      | > 9.9.0      | > N/A        | > 9.8.0\*    | > N/A              |
+-------------+--------------+--------------+--------------+--------------+--------------------+
| Ogre        | > 1.10\*                                                  | > N/A              |
+-------------+--------------+--------------+--------------+--------------+--------------------+
| OpenCV      | > 3.2.0      | > 4.1.0      | > 3.4.6\*    | > 3.2.0      | 4.1.0 /            |
|             |              |              |              |              | 3.2.0\*\*\*\*      |
+-------------+--------------+--------------+--------------+--------------+--------------------+
| OpenSSL     | > 1.1.0g     | > 1.0.2r     | > 1.0.2r     | > 1.1.1c     | 1.1.1d /           |
|             |              |              |              |              | 1.1.1b\*\*\*\*     |
+-------------+--------------+--------------+--------------+--------------+--------------------+
| Poco        | > 1.8.0      | > 1.9.0      | > 1.8.0\*    | > 1.9.0      | > 1.9.4            |
+-------------+--------------+--------------+--------------+--------------+--------------------+
| Python      | > 3.6.5      | > 3.7.3      | > 3.7.3      | > 3.7.3      | 3.8.2 /            |
|             |              |              |              |              | 3.7.5\*\*\*\*      |
+-------------+--------------+--------------+--------------+--------------+--------------------+
| Qt          | > 5.9.5      | > 5.12.3     | > 5.10.0     | > 5.11.3     | 5.14.1 /           |
|             |              |              |              |              | 5.12.5\*\*\*\*     |
+-------------+--------------+--------------+--------------+--------------+--------------------+
|                            | > **Linux only**                                                |
+-------------+--------------+--------------+--------------+--------------+--------------------+
| PCL         | > 1.8.1      | > N/A        | > N/A        | > 1.9.1      | > 1.8.1            |
+-------------+--------------+--------------+--------------+--------------+--------------------+
| > **RMW DDS Middleware Providers**                                                           |
+-------------+--------------------------------------------+-----------------------------------+
| Connext DDS | > 5.3.1\*\*\*                              | > N/A                             |
+-------------+--------------------------------------------+-----------------------------------+
| Cyclone DDS | > 0.7.x (Coquette)                                                             |
+-------------+--------------------------------------------------------------------------------+
| > Fast-RTPS | > 1.9.0                                                                        |
+-------------+-----------------------------------------------------------+--------------------+
| OpenSplice  | > 6.9.190705OSS                                           | > N/A              |
+-------------+-----------------------------------------------------------+--------------------+

\" \* \" means that this is not the upstream version (available on the
official Operating System repositories) but a package distributed by
OSRF or the community (package built and distributed on custom
repositories).

\" \*\* \" Rolling distributions will see multiple version changes of
these dependencies during their lifetime. The versions shown for
OpenEmbedded are those provided by the 3.1 Dunfell release series; the
versions provided by the other supported release series are listed here:
<https://github.com/ros/meta-ros/wiki/Package-Version-Differences> .
Note that the OpenEmbedded releases series for which a ROS distro has
support will change during its support time frame, as per the
OpenEmbedded support policy shown here:
<https://github.com/ros/meta-ros/wiki/Policies#openembedded-release-series-support>
. However, it will always be supported by least one stable OpenEmbedded
release series.

\" \*\*\* \" It is anticipated that this will be increased to Connext
DDS 6.0.0 pending migration patches[^8].

\" \*\*\*\* \" webOS OSE provides this different version.

This document only captures the version at the first release of a ROS
distribution and will not be updated as the dependencies move forward.
These versions are thus a low watermark.

Package manager use for dependencies:

- Ubuntu, Debian: apt
- MacOS: Homebrew, pip
- Windows: Chocolatey, pip
- OpenEmbedded: opkg

Build System Support:

- ament_cmake
- cmake
- setuptools

Foxy Fitzroy (May 2020 - May 2023)
--------------------------------------

Targeted platforms:

+--------------+-------------------+--------------+--------------+----------+--------------+
| Architecture | Ubuntu Focal      | MacOS Mojave | Windows 10   | Debian   | OpenEmbedded |
|              | (20.04)           | (10.14)      | (VS2019)     | Buster   | / webOS OSE  |
|              |                   |              |              | (10)     |              |
+==============+===================+==============+==============+==========+==============+
| > amd64      | > Tier 1          | > Tier 1     | > Tier 1     | > Tier 3 |              |
|              | > \[d\]\[a\]\[s\] | > \[a\]\[s\] | > \[a\]\[s\] | > \[s\]  |              |
+--------------+-------------------+--------------+--------------+----------+--------------+
| > arm64      | > Tier 1          |              |              | > Tier 3 | > Tier 3     |
|              | > \[d\]\[a\]\[s\] |              |              | > \[s\]  | > \[s\]      |
+--------------+-------------------+--------------+--------------+----------+--------------+
| > arm32      | > Tier 3 \[s\]    |              |              | > Tier 3 | > Tier 3     |
|              |                   |              |              | > \[s\]  | > \[s\]      |
+--------------+-------------------+--------------+--------------+----------+--------------+

The following indicators show what delivery mechanisms are available for
each platform.

\" \[d\] \" Debian packages will be provided for this platform for
packages submitted to the rosdistro.

\" \[a\] \" Binary releases are provided as a single archive per
platform containing all packages in the Foxy ROS 2 repos file[^9].

\" \[s\] \" Compilation from source.

Middleware Implementation Support:

  ----------------------------------------------------------------------------------------
  Middleware Library         Middleware      Support   Platforms       Architectures
                             Provider        Level                     
  -------------------------- --------------- --------- --------------- -------------------
  rmw_fastrtps_cpp\*         eProsima        Tier 1    All Platforms   All Architectures
                             Fast-RTPS                                 

  rmw_cyclonedds_cpp         Eclipse Cyclone Tier 1    All Platforms   All Architectures
                             DDS                                       

  rmw_connext_cpp            RTI Connext     Tier 1    All Platforms   All Architectures
                                                       except Debian   except arm64/arm32
                                                       and             
                                                       OpenEmbedded    

  rmw_fastrtps_dynamic_cpp   eProsima        Tier 2    All Platforms   All Architectures
                             Fast-RTPS                                 

  rmw_gurumdds_cpp           GurumNetworks   Tier 3    Ubuntu and      All Architectures
                             GurumDDS                  Windows         except arm32
  ----------------------------------------------------------------------------------------

\" \* \" means default RMW implementation.

Middleware implementation support is dependent upon the platform support
tier. For example a Tier 1 middleware implementation on a Tier 2
platform can only receive Tier 2 support.

Minimum language requirements:

- C++14
- Python 3.7

Dependency Requirements:

+-------------+--------------------------------------------+---------------------------------+
|             | > Required Support                         | > Recommended Support           |
+-------------+--------------+--------------+--------------+--------------+------------------+
| Package     | > Ubuntu     | > MacOS\*\*  | > Windows    | Debian       | OpenEmbedded\*\* |
|             | > Focal      |              | > 10\*\*     | Buster       |                  |
+=============+==============+==============+==============+==============+==================+
| CMake       | > 3.16.3     | > 3.14.4     | > 3.14.4     | > 3.13.4     | 3.16.1 /         |
|             |              |              |              |              | 3.12.2\*\*\*\*   |
+-------------+--------------+--------------+--------------+--------------+------------------+
| EmPY        | > 3.3.2                                                                      |
+-------------+--------------+--------------+--------------+--------------+------------------+
| Gazebo      | > 11.0.0\*   | > 11.0.0     | > N/A        | > 11.0.0\*   | > N/A            |
+-------------+--------------+--------------+--------------+--------------+------------------+
| Ignition    | > Citadel\*                 | > N/A        | > Citadel\*  | > N/A            |
+-------------+-----------------------------+--------------+--------------+------------------+
| Ogre        | > 1.10\*                                                  | > N/A            |
+-------------+--------------+--------------+--------------+--------------+------------------+
| OpenCV      | > 4.2.0      | > 4.2.0      | > 3.4.6\*    | > 3.2.0      | > 4.1.0 /        |
|             |              |              |              |              | > 3.2.0\*\*\*\*  |
+-------------+--------------+--------------+--------------+--------------+------------------+
| OpenSSL     | > 1.1.1d     | > 1.1.1f     | > 1.1.1f     | > 1.1.1d     | 1.1.1d /         |
|             |              |              |              |              | 1.1.1b\*\*\*\*   |
+-------------+--------------+--------------+--------------+--------------+------------------+
| Poco        | > 1.9.2      | > 1.9.0      | > 1.8.0\*    | > 1.9.0      | > 1.9.4          |
+-------------+--------------+--------------+--------------+--------------+------------------+
| Python      | > 3.8.0      | > 3.8.2      | > 3.8.0      | > 3.7.3      | > 3.8.2 /        |
|             |              |              |              |              | > 3.7.5\*\*\*\*  |
+-------------+--------------+--------------+--------------+--------------+------------------+
| Qt          | > 5.12.5     | > 5.12.3     | > 5.10.0     | > 5.11.3     | 5.14.1 /         |
|             |              |              |              |              | 5.12.5\*\*\*\*   |
+-------------+--------------+--------------+--------------+--------------+------------------+
|                            | > **Linux only**                                              |
+-------------+--------------+--------------+--------------+--------------+------------------+
| PCL         | > 1.10.0     | > N/A        | > N/A        | > 1.9.1      | > 1.10.0         |
+-------------+--------------+--------------+--------------+--------------+------------------+
| > **RMW DDS Middleware Providers**                                                         |
+-------------+--------------------------------------------+---------------------------------+
| Connext DDS | > 5.3.1                                    | > N/A                           |
+-------------+--------------------------------------------+---------------------------------+
| Cyclone DDS | > 0.7.x (Coquette)                                                           |
+-------------+------------------------------------------------------------------------------+
| > Fast-RTPS | > 2.0.x                                                                      |
+-------------+--------------+--------------+--------------+---------------------------------+
| Gurum DDS   | > 2.7.x      | > N/A        | > 2.7.x      | > N/A                           |
+-------------+--------------+--------------+--------------+---------------------------------+

\" \* \" means that this is not the upstream version (available on the
official Operating System repositories) but a package distributed by
OSRF or the community (package built and distributed on custom
repositories).

\" \*\* \" Rolling distributions will see multiple version changes of
these dependencies during their lifetime. The versions shown for
OpenEmbedded are those provided by the 3.1 Dunfell release series; the
versions provided by the other supported release series are listed here:
<https://github.com/ros/meta-ros/wiki/Package-Version-Differences> .
Note that the OpenEmbedded releases series for which a ROS distro has
support will change during its support time frame, as per the
OpenEmbedded support policy shown here:
<https://github.com/ros/meta-ros/wiki/Policies#openembedded-release-series-support>
. However, it will always be supported by least one stable OpenEmbedded
release series.

\" \*\*\*\* \" webOS OSE provides this different version.

This document only captures the version at the first release of a ROS
distribution and will not be updated as the dependencies move forward.
These versions are thus a low watermark.

Package manager use for dependencies:

- Ubuntu, Debian: apt
- MacOS: Homebrew, pip
- Windows: Chocolatey, pip
- OpenEmbedded: opkg

Build System Support:

- ament_cmake
- cmake
- setuptools


Galactic Geochelone (May 2021 - November 2022)
----------------------------------------------

Targeted platforms:

+--------------+-----------------+------------+-----------------+-------+----------+--------------+
| Architecture | Ubuntu Focal    | Windows 10 | RHEL 8          | macOS | Debian   | OpenEmbedded |
|              | (20.04)         | (VS2019)   |                 |       | Bullseye | / webOS OSE  |
|              |                 |            |                 |       | (11)     |              |
+==============+=================+============+=================+=======+==========+==============+
| > amd64      | Tier 1          | Tier 1     | Tier 2          | Tier  | > Tier 3 |              |
|              | \[d\]\[a\]\[s\] | \[a\]\[s\] | \[d\]\[a\]\[s\] | 3     | > \[s\]  |              |
|              |                 |            |                 | \[s\] |          |              |
+--------------+-----------------+------------+-----------------+-------+----------+--------------+
| > arm64      | Tier 1          |            |                 |       | > Tier 3 | > Tier 3     |
|              | \[d\]\[a\]\[s\] |            |                 |       | > \[s\]  | > \[s\]      |
+--------------+-----------------+------------+-----------------+-------+----------+--------------+
| > arm32      | > Tier 3 \[s\]  |            |                 |       | > Tier 3 | > Tier 3     |
|              |                 |            |                 |       | > \[s\]  | > \[s\]      |
+--------------+-----------------+------------+-----------------+-------+----------+--------------+

The following indicators show what delivery mechanisms are available for
each platform.

\" \[d\] \" Distribution-specific (Debian, RPM, etc.) packages will be
provided for this platform for packages submitted to the rosdistro.

\" \[a\] \" Binary releases are provided as a single archive per
platform containing all packages in the Galactic ROS 2 repos file[^10].

\" \[s\] \" Compilation from source.

Middleware Implementation Support:

  --------------------------------------------------------------------------------------
  Middleware Library         Middleware      Support   Platforms       Architectures
                             Provider        Level                     
  -------------------------- --------------- --------- --------------- -----------------
  rmw_cyclonedds_cpp\*       Eclipse Cyclone Tier 1    All Platforms   All Architectures
                             DDS                                       

  rmw_fastrtps_cpp           eProsima        Tier 1    All Platforms   All Architectures
                             Fast-DDS                                  

  rmw_connextdds             RTI Connext     Tier 1    Ubuntu,         All Architectures
                                                       Windows, and    except arm64
                                                       macOS           

  rmw_fastrtps_dynamic_cpp   eProsima        Tier 2    All Platforms   All Architectures
                             Fast-DDS                                  

  rmw_gurumdds_cpp           GurumNetworks   Tier 3    Ubuntu and      All Architectures
                             GurumDDS                  Windows         except arm32
  --------------------------------------------------------------------------------------

\" \* \" means default RMW implementation.

Middleware implementation support is dependent upon the platform support
tier. For example a Tier 1 middleware implementation on a Tier 2
platform can only receive Tier 2 support.

Minimum language requirements:

- C++17
- Python 3.6

Dependency Requirements:

+--------------+-----------------------------+-----------------------------------------------------------------+
|              | > Required Support          | > Recommended Support                                           |
+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| Package      | > Ubuntu     | > Windows    | > RHEL 8     | > macOS\*\*  | Debian       | > OpenEmbedded\*\* |
|              | > Focal      | > 10\*\*     |              |              | Bullseye     |                    |
+==============+==============+==============+==============+==============+==============+====================+
| CMake        | > 3.16.3     | > 3.19.1     | > 3.18.2     | > 3.14.4     | > 3.18.4     | 3.16.1 /           |
|              |              |              |              |              |              | 3.12.2\*\*\*\*     |
+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| EmPY         | > 3.3.2                                                                                       |
+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| Gazebo       | > 11.0.0\*   | > N/A        | > N/A        | > 11.0.0     | > 11.0.0\*   | > N/A              |
+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| Ignition     | > Edifice\*  | > N/A        | > N/A        | > Edifice\*  | > Edifice\*  | > N/A              |
+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| Ogre         | > 1.10\*                                                                 | > N/A              |
+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| OpenCV       | > 4.2.0      | > 3.4.6\*    | > 3.4.6      | > 4.2.0      | > 4.5.1      | > 4.1.0 /          |
|              |              |              |              |              |              | > 3.2.0\*\*\*\*    |
+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| OpenSSL      | > 1.1.1d     | > 1.1.1i     | > 1.1.1g     | > 1.1.1f     | > 1.1.1i     | 1.1.1d /           |
|              |              |              |              |              |              | 1.1.1b\*\*\*\*     |
+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| Python       | > 3.8.0      | > 3.8.3      | > 3.6.8      | > 3.8.2      | > 3.9.1      | > 3.8.2 /          |
|              |              |              |              |              |              | > 3.7.5\*\*\*\*    |
+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| Qt           | > 5.12.5     | > 5.12.10    | > 5.12.5     | > 5.12.3     | > 5.15.2     | 5.14.1 /           |
|              |              |              |              |              |              | 5.12.5\*\*\*\*     |
+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
|                             | > **Linux only**                                                               |
+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| PCL          | > 1.10.0     | > N/A        | > 1.11.1     | > N/A        | > 1.11.1     | > 1.10.0           |
+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| > **RMW DDS Middleware Providers**                                                                           |
+--------------+-----------------------------------------------------------------------------------------------+
| Cyclone DDS  | > 0.8.x (Réplique)                                                                            |
+--------------+-----------------------------------------------------------------------------------------------+
| Fast-DDS     | > 2.3.x                                                                                       |
+--------------+-----------------------------+--------------+--------------+-----------------------------------+
| Connext DDS  | > 5.3.1                     | > N/A        | > 5.3.1      | > N/A                             |
+--------------+-----------------------------+--------------+--------------+-----------------------------------+
| Gurum DDS    | > 2.7.x                     | > N/A                                                           |
+--------------+-----------------------------+-----------------------------------------------------------------+

\" \* \" means that this is not the upstream version (available on the
official Operating System repositories) but a package distributed by
OSRF or the community (package built and distributed on custom
repositories).

\" \*\* \" Rolling distributions will see multiple version changes of
these dependencies during their lifetime. The versions shown for
OpenEmbedded are those provided by the 3.1 Dunfell release series; the
versions provided by the other supported release series are listed here:
<https://github.com/ros/meta-ros/wiki/Package-Version-Differences> .
Note that the OpenEmbedded releases series for which a ROS distro has
support will change during its support time frame, as per the
OpenEmbedded support policy shown here:
<https://github.com/ros/meta-ros/wiki/Policies#openembedded-release-series-support>
. However, it will always be supported by least one stable OpenEmbedded
release series.

\" \*\*\*\* \" webOS OSE provides this different version.

This document only captures the version at the first release of a ROS
distribution and will not be updated as the dependencies move forward.
These versions are thus a low watermark.

Package manager use for dependencies:

- Ubuntu, Debian: apt
- Windows: Chocolatey, pip
- macOS: Homebrew, pip
- RHEL: dnf
- OpenEmbedded: opkg

Build System Support:

- ament_cmake
- cmake
- setuptools

Humble Hawksbill (May 2022 - May 2027)
--------------------------------------

Targeted platforms:

+--------------+-----------------+------------+-----------------+---------+-------+----------+--------------+
| Architecture | Ubuntu Jammy    | Windows 10 | RHEL 8          | Ubuntu  | macOS | Debian   | OpenEmbedded |
|              | (22.04)         | (VS2019)   |                 | Focal   |       | Bullseye | / Yocto      |
|              |                 |            |                 | (20.04) |       | (11)     | Project      |
+==============+=================+============+=================+=========+=======+==========+==============+
| > amd64      | Tier 1          | Tier 1     | Tier 2          | Tier 3  | Tier  | > Tier 3 | > Tier 3     |
|              | \[d\]\[a\]\[s\] | \[a\]\[s\] | \[d\]\[a\]\[s\] | \[s\]   | 3     | > \[s\]  | > \[s\]      |
|              |                 |            |                 |         | \[s\] |          |              |
+--------------+-----------------+------------+-----------------+---------+-------+----------+--------------+
| > arm64      | Tier 1          |            |                 | Tier 3  |       | > Tier 3 | > Tier 3     |
|              | \[d\]\[a\]\[s\] |            |                 | \[s\]   |       | > \[s\]  | > \[s\]      |
+--------------+-----------------+------------+-----------------+---------+-------+----------+--------------+
| > arm32      | > Tier 3 \[s\]  |            |                 | Tier 3  |       | > Tier 3 | > Tier 3     |
|              |                 |            |                 | \[s\]   |       | > \[s\]  | > \[s\]      |
+--------------+-----------------+------------+-----------------+---------+-------+----------+--------------+

The following indicators show what delivery mechanisms are available for
each platform.

\" \[d\] \" Distribution-specific (Debian, RPM, etc.) packages will be
provided for this platform for packages submitted to the rosdistro.

\" \[a\] \" Binary releases are provided as a single archive per
platform containing all packages in the Humble ROS 2 repos file[^11].

\" \[s\] \" Compilation from source.

Middleware Implementation Support:

  --------------------------------------------------------------------------------------
  Middleware Library         Middleware      Support   Platforms       Architectures
                             Provider        Level                     
  -------------------------- --------------- --------- --------------- -----------------
  rmw_fastrtps_cpp\*         eProsima        Tier 1    All Platforms   All Architectures
                             Fast-DDS                                  

  rmw_cyclonedds_cpp         Eclipse Cyclone Tier 1    All Platforms   All Architectures
                             DDS                                       

  rmw_connextdds             RTI Connext     Tier 1    Ubuntu,         All Architectures
                                                       Windows, and    except arm64
                                                       macOS           

  rmw_fastrtps_dynamic_cpp   eProsima        Tier 2    All Platforms   All Architectures
                             Fast-DDS                                  

  rmw_gurumdds_cpp           GurumNetworks   Tier 3    Ubuntu and      All Architectures
                             GurumDDS                  Windows         except arm32
  --------------------------------------------------------------------------------------

\" \* \" means default RMW implementation.

Middleware implementation support is dependent upon the platform support
tier. For example a Tier 1 middleware implementation on a Tier 2
platform can only receive Tier 2 support.

Minimum language requirements:

- C++17
- Python 3.6

Dependency Requirements:

+------------+-----------------------------+--------------------------------------------------------------------------------+
|            | > Required Support          | > Recommended Support                                                          |
+------------+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| Package    | > Ubuntu     | > Windows    | > RHEL 8     | > Ubuntu     | > macOS\*\*  | Debian       | > OpenEmbedded\*\* |
|            | > Jammy      | > 10\*\*     |              | > Focal      |              | Bullseye     |                    |
+============+==============+==============+==============+==============+==============+==============+====================+
| CMake      | > 3.22.1     | > 3.22.0     | > 3.20.2     | > 3.16.3     | > 3.14.4     | > 3.18.4     | 3.22.3 /           |
|            |              |              |              |              |              |              | 3.16.5\*\*\*       |
+------------+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| EmPY       | > 3.3.4      | > 3.3.2                                                                                       |
+------------+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| Gazebo     | > 11.x.x\*   | > N/A        | > N/A        | > 11.0.0\*   | > 11.x.x     | > 11.x.x\*   | > N/A              |
| Classic    |              |              |              |              |              |              |                    |
+------------+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| Gazebo     | > Fortress\* | > N/A        | > N/A        | > Fortress\* | > Fortress\* | > Fortress\* | > N/A              |
| (Ignition) |              |              |              |              |              |              |                    |
+------------+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| NumPy      | > 1.21.5     | > 1.18.4     | > 1.14.3     | > 1.17.4     | > 1.18.4     | > 1.19.5     | > N/A              |
+------------+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| Ogre       | > 1.12.1\*                                                                              | > N/A              |
+------------+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| OpenCV     | > 4.5.4      | > 3.4.6\*    | > 3.4.6      | > 4.2.0      | > 4.2.0      | > 4.5.1      | > 4.1.0 /          |
|            |              |              |              |              |              |              | > 3.2.0\*\*\*      |
+------------+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| OpenSSL    | > 1.1.1l     | > 1.1.1l     | > 1.1.1k     | > 1.1.1d     | > 1.1.1f     | > 1.1.1i     | 1.1.1d /           |
|            |              |              |              |              |              |              | 1.1.1b\*\*\*       |
+------------+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| Python     | > 3.10.4     | > 3.8.3      | > 3.6.8      | > 3.8.0      | > 3.8.2      | > 3.9.1      | > 3.8.2 /          |
|            |              |              |              |              |              |              | > 3.7.5\*\*\*      |
+------------+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| Qt         | > 5.15.3     | > 5.12.12    | > 5.15.2     | > 5.12.5     | > 5.12.3     | > 5.15.2     | 5.14.1 /           |
|            |              |              |              |              |              |              | 5.12.5\*\*\*       |
+------------+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
|                           | > **Linux only**                                                                              |
+------------+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| PCL        | > 1.12.1     | > N/A        | > 1.11.1     | > 1.10.0     | > N/A        | > 1.11.1     | > 1.10.0           |
+------------+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| > **RMW DDS Middleware Providers**                                                                                        |
+------------+--------------------------------------------------------------------------------------------------------------+
| Cyclone    | > 0.9.x (Papillons)                                                                                          |
| DDS        |                                                                                                              |
+------------+--------------------------------------------------------------------------------------------------------------+
| Fast-DDS   | > 2.6.x                                                                                                      |
+------------+-----------------------------+--------------+-----------------------------+-----------------------------------+
| Connext    | > 6.0.1                     | > N/A        | > 6.0.1                     | > N/A                             |
| DDS        |                             |              |                             |                                   |
+------------+-----------------------------+--------------+--------------+--------------+-----------------------------------+
| Gurum DDS  | > 2.7.x                     | > N/A        | > 2.7.x      | > N/A                                            |
+------------+-----------------------------+--------------+--------------+--------------------------------------------------+

\" \* \" means that this is not the upstream version (available on the
official Operating System repositories) but a package distributed by
OSRF or the community (package built and distributed on custom
repositories).

\" \*\* \" means that the dependency may see multiple version changes,
because the dependency uses a package manager that continually updates
the dependency without a stable API.

\" \*\*\* \" webOS OSE provides this different version.

This document only captures the version at the first release of a ROS
distribution and will not be updated as the dependencies move forward.
These versions are thus a low watermark.

Package manager use for dependencies:

- Ubuntu, Debian: apt
- Windows: Chocolatey, pip
- macOS: Homebrew, pip
- RHEL: dnf
- OpenEmbedded: opkg

Build System Support:

- ament_cmake
- cmake
- setuptools

Iron Irwini (May 2023 - November 2024)
--------------------------------------

Targeted platforms:

+--------------+-----------------+------------+-----------------+---------+----------+--------------+
| Architecture | Ubuntu Jammy    | Windows 10 | RHEL 9          | > macOS | Debian   | OpenEmbedded |
|              | (22.04)         | (VS2019)   |                 |         | Bullseye | / Yocto      |
|              |                 |            |                 |         | (11)     | Project      |
+==============+=================+============+=================+=========+==========+==============+
| > amd64      | Tier 1          | Tier 1     | Tier 2          | > Tier  | > Tier 3 | > Tier 3     |
|              | \[d\]\[a\]\[s\] | \[a\]\[s\] | \[d\]\[a\]\[s\] | > 3     | > \[s\]  | > \[s\]      |
|              |                 |            |                 | > \[s\] |          |              |
+--------------+-----------------+------------+-----------------+---------+----------+--------------+
| > arm64      | Tier 1          |            |                 |         | > Tier 3 | > Tier 3     |
|              | \[d\]\[a\]\[s\] |            |                 |         | > \[s\]  | > \[s\]      |
+--------------+-----------------+------------+-----------------+---------+----------+--------------+
| > arm32      | > Tier 3 \[s\]  |            |                 |         | > Tier 3 | > Tier 3     |
|              |                 |            |                 |         | > \[s\]  | > \[s\]      |
+--------------+-----------------+------------+-----------------+---------+----------+--------------+

The following indicators show what delivery mechanisms are available for
each platform.

\" \[d\] \" Distribution-specific (Debian, RPM, etc.) packages will be
provided for this platform for packages submitted to the rosdistro.

\" \[a\] \" Binary releases are provided as a single archive per
platform containing all packages in the Iron ROS 2 repos file[^12].

\" \[s\] \" Compilation from source.

Middleware Implementation Support:

  --------------------------------------------------------------------------------------
  Middleware Library         Middleware      Support   Platforms       Architectures
                             Provider        Level                     
  -------------------------- --------------- --------- --------------- -----------------
  rmw_fastrtps_cpp\*         eProsima        Tier 1    All Platforms   All Architectures
                             Fast-DDS                                  

  rmw_cyclonedds_cpp         Eclipse Cyclone Tier 1    All Platforms   All Architectures
                             DDS                                       

  rmw_connextdds             RTI Connext     Tier 1    Ubuntu,         All Architectures
                                                       Windows, and    except arm64
                                                       macOS           

  rmw_fastrtps_dynamic_cpp   eProsima        Tier 2    All Platforms   All Architectures
                             Fast-DDS                                  

  rmw_gurumdds_cpp           GurumNetworks   Tier 3    Ubuntu and      All Architectures
                             GurumDDS                  Windows         except arm32
  --------------------------------------------------------------------------------------

\" \* \" means default RMW implementation.

Middleware implementation support is dependent upon the platform support
tier. For example a Tier 1 middleware implementation on a Tier 2
platform can only receive Tier 2 support.

Minimum language requirements:

- C++17
- Python 3.8

Dependency Requirements:

+--------------+-----------------------------+-----------------------------------------------------------------+
|              | > Required Support          | > Recommended Support                                           |
+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| Package      | > Ubuntu     | > Windows    | > RHEL 9     | > macOS\*\*  | Debian       | > OpenEmbedded\*\* |
|              | > Jammy      | > 10\*\*     |              |              | Bullseye     |                    |
+==============+==============+==============+==============+==============+==============+====================+
| CMake        | > 3.22.1     | > 3.22.0     | > 3.20.2     | > 3.14.4     | > 3.18.4     | 3.22.3 /           |
|              |              |              |              |              |              | 3.16.5\*\*\*       |
+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| EmPY         | > 3.3.4      | > 3.3.2      | > 3.3.4      | > 3.3.2                                          |
+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| Gazebo       | > 11.x.x\*   | > N/A        | > N/A        | > 11.x.x     | > 11.x.x\*   | > N/A              |
| Classic      |              |              |              |              |              |                    |
+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| Gazebo       | > Fortress\* | > N/A        | > N/A        | > Fortress\* | > Fortress\* | > N/A              |
| (Ignition)   |              |              |              |              |              |                    |
+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| NumPy        | > 1.21.5     | > 1.18.4     | > 1.20.1     | > 1.18.4     | > 1.19.5     | > N/A              |
+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| Ogre         | > 1.12.1\*                                                               | > N/A              |
+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| OpenCV       | > 4.5.4      | > 3.4.6\*    | > 4.6.0      | > 4.2.0      | > 4.5.1      | > 4.1.0 /          |
|              |              |              |              |              |              | > 3.2.0\*\*\*      |
+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| OpenSSL      | > 3.0.2      | > 1.1.1l     | > 3.0.1      | > 1.1.1f     | > 1.1.1i     | 1.1.1d /           |
|              |              |              |              |              |              | 1.1.1b\*\*\*       |
+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| Python       | > 3.10.6     | > 3.8.3      | > 3.9.14     | > 3.10.8     | > 3.9.1      | > 3.8.2 /          |
|              |              |              |              |              |              | > 3.7.5\*\*\*      |
+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| Qt           | > 5.15.3     | > 5.12.12    | > 5.15.3     | > 5.12.3     | > 5.15.2     | 5.14.1 /           |
|              |              |              |              |              |              | 5.12.5\*\*\*       |
+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
|                             | > **Linux only**                                                               |
+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| PCL          | > 1.12.1     | > N/A        | > 1.12.0     | > N/A        | > 1.11.1     | > 1.10.0           |
+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| > **RMW DDS Middleware**                                                                                     |
+--------------+-----------------------------------------------------------------------------------------------+
| Cyclone DDS  | > 0.9                                                                                         |
+--------------+-----------------------------------------------------------------------------------------------+
| Fast-DDS     | > 2.8                                                                                         |
+--------------+-----------------------------------------------------------+-----------------------------------+
| Connext DDS  | > 6.0.1                                                   | > N/A                             |
+--------------+-----------------------------+-----------------------------+-----------------------------------+
| Gurum DDS    | > 2.8.x                     | > N/A                                                           |
+--------------+-----------------------------+-----------------------------------------------------------------+

\" \* \" means that this is not the upstream version (available on the
official Operating System repositories) but a package distributed by
OSRF or the community (package built and distributed on custom
repositories).

\" \*\* \" means that the dependency may see multiple version changes,
because the dependency uses a package manager that continually updates
the dependency without a stable API.

\" \*\*\* \" webOS OSE provides this different version.

This document only captures the version at the first release of a ROS
distribution and will not be updated as the dependencies move forward.
These versions are thus a low watermark.

Package manager use for dependencies:

- Ubuntu, Debian: apt
- Windows: Chocolatey, pip
- macOS: Homebrew, pip
- RHEL: dnf
- OpenEmbedded: opkg

Build System Support:

- ament_cmake
- cmake
- setuptools

Jazzy Jalisco (May 2024 - May 2029)
-----------------------------------


Targeted platforms:

+--------------+-----------------+------------+-----------------+---------+---------+----------+--------------+
| Architecture | Ubuntu Noble    | Windows 10 | RHEL 9          | Ubuntu  | > macOS | Debian   | OpenEmbedded |
|              | (24.04)         | (VS2019)   |                 | Jammy   |         | Bookworm | / Yocto      |
|              |                 |            |                 | (22.04) |         | (12)     | Project      |
+==============+=================+============+=================+=========+=========+==========+==============+
| > amd64      | Tier 1          | Tier 1     | Tier 2          | > Tier  | > Tier  | > Tier 3 | > Tier 3     |
|              | \[d\]\[a\]\[s\] | \[a\]\[s\] | \[d\]\[a\]\[s\] | > 3     | > 3     | > \[s\]  | > \[s\]      |
|              |                 |            |                 | > \[s\] | > \[s\] |          |              |
+--------------+-----------------+------------+-----------------+---------+---------+----------+--------------+
| > arm64      | Tier 1          |            |                 |         |         | > Tier 3 | > Tier 3     |
|              | \[d\]\[a\]\[s\] |            |                 |         |         | > \[s\]  | > \[s\]      |
+--------------+-----------------+------------+-----------------+---------+---------+----------+--------------+
| > arm32      | > Tier 3 \[s\]  |            |                 |         |         | > Tier 3 | > Tier 3     |
|              |                 |            |                 |         |         | > \[s\]  | > \[s\]      |
+--------------+-----------------+------------+-----------------+---------+---------+----------+--------------+

The following indicators show what delivery mechanisms are available for
each platform.

\" \[d\] \" Distribution-specific (Debian, RPM, etc.) packages will be
provided for this platform for packages submitted to the rosdistro.

\" \[a\] \" Binary releases are provided as a single archive per
platform containing all packages in the Jazzy ROS 2 repos file[^13].

\" \[s\] \" Compilation from source.

Middleware Implementation Support:

  --------------------------------------------------------------------------------------
  Middleware Library         Middleware      Support   Platforms       Architectures
                             Provider        Level                     
  -------------------------- --------------- --------- --------------- -----------------
  rmw_fastrtps_cpp\*         eProsima        Tier 1    All Platforms   All Architectures
                             Fast-DDS                                  

  rmw_cyclonedds_cpp         Eclipse Cyclone Tier 1    All Platforms   All Architectures
                             DDS                                       

  rmw_connextdds             RTI Connext     Tier 1    Ubuntu,         All Architectures
                                                       Windows, and    except arm64
                                                       macOS           

  rmw_fastrtps_dynamic_cpp   eProsima        Tier 2    All Platforms   All Architectures
                             Fast-DDS                                  

  rmw_gurumdds_cpp           GurumNetworks   Tier 3    Ubuntu and      All Architectures
                             GurumDDS                  Windows         except arm32
  --------------------------------------------------------------------------------------

\" \* \" means default RMW implementation.

Middleware implementation support is dependent upon the platform support
tier. For example a Tier 1 middleware implementation on a Tier 2
platform can only receive Tier 2 support.

Minimum language requirements:

- C++17
- Python 3.8

Dependency Requirements:

+-----------+----------------------------+-------------------------------------------------------------------------------+
|           | > Required Support         | > Recommended Support                                                         |
+-----------+--------------+-------------+-------------+--------------+--------------+--------------+--------------------+
| Package   | > Ubuntu     | > Windows   | > RHEL 9    | > Ubuntu     | > macOS\*\*  | Debian       | > OpenEmbedded\*\* |
|           | > Noble      | > 10\*\*    |             | > Jammy      |              | Bookworm     |                    |
+===========+==============+=============+=============+==============+==============+==============+====================+
| CMake     | > 3.28.3     | > 3.22.0    | > 3.20.2    | > 3.22.1     | > 3.20.0     | > 3.25.1     | > 3.22.3           |
+-----------+--------------+-------------+-------------+--------------+--------------+--------------+--------------------+
| EmPY      | > 3.3.4      | > 3.3.2     | > 3.3.4                                                                       |
+-----------+--------------+-------------+-------------+--------------+--------------+--------------+--------------------+
| Gazebo    | > Harmonic\* | > N/A       | > N/A       | > Harmonic\* | > Harmonic\* | > Harmonic\* | > N/A              |
+-----------+--------------+-------------+-------------+--------------+--------------+--------------+--------------------+
| NumPy     | > 1.26.4     | > 1.18.4    | > 1.20.1    | > 1.21.5     | > 1.18.4     | > 1.24.2     | > N/A              |
+-----------+--------------+-------------+-------------+--------------+--------------+--------------+--------------------+
| Ogre      | > 1.12.10                                                                             | > N/A              |
+-----------+--------------+-------------+-------------+--------------+--------------+--------------+--------------------+
| OpenCV    | > 4.6.0      | > 3.4.6\*   | > 4.6.0     | > 4.5.4      | > 4.2.0      | > 4.6.0      | > 4.1.0 /          |
|           |              |             |             |              |              |              | > 3.2.0\*\*\*      |
+-----------+--------------+-------------+-------------+--------------+--------------+--------------+--------------------+
| OpenSSL   | > 3.0.13     | > 1.1.1l    | > 3.0.7     | > 1.1.1l     | > 1.1.1f     | > 3.0.11     | 1.1.1d /           |
|           |              |             |             |              |              |              | 1.1.1b\*\*\*       |
+-----------+--------------+-------------+-------------+--------------+--------------+--------------+--------------------+
| Python    | > 3.12.3     | > 3.8.3     | > 3.9.16    | > 3.10.4     | > 3.10.8     | > 3.11.2     | > 3.8.2 /          |
|           |              |             |             |              |              |              | > 3.7.5\*\*\*      |
+-----------+--------------+-------------+-------------+--------------+--------------+--------------+--------------------+
| Qt        | > 5.15.10    | > 5.12.12   | > 5.15.3    | > 5.15.3     | > 5.12.3     | > 5.15.8     | 5.14.1 /           |
|           |              |             |             |              |              |              | 5.12.5\*\*\*       |
+-----------+--------------+-------------+-------------+--------------+--------------+--------------+--------------------+
|                          | > **Linux only**                                                                            |
+-----------+--------------+-------------+-------------+--------------+--------------+--------------+--------------------+
| PCL       | > 1.14.0     | > N/A       | > 1.12.0    | > 1.12.1     | > N/A        | > 1.13.0     | > 1.10.0           |
+-----------+--------------+-------------+-------------+--------------+--------------+--------------+--------------------+
| > **RMW DDS Middleware**                                                                                               |
+-----------+------------------------------------------------------------------------------------------------------------+
| Cyclone   | > 0.10.4                                                                                                   |
| DDS       |                                                                                                            |
+-----------+------------------------------------------------------------------------------------------------------------+
| Fast-DDS  | > 2.14.0                                                                                                   |
+-----------+------------------------------------------------------------------------+-----------------------------------+
| Connext   | > 6.0.1                                                                | > N/A                             |
| DDS       |                                                                        |                                   |
+-----------+----------------------------+-------------------------------------------+-----------------------------------+
| Gurum DDS | > 4.2.0                    | > N/A                                                                         |
+-----------+----------------------------+-------------------------------------------------------------------------------+

\" \* \" means that this is not the upstream version (available on the
official Operating System repositories) but a package distributed by
OSRF or the community (package built and distributed on custom
repositories).

\" \*\* \" means that the dependency may see multiple version changes,
because the dependency uses a package manager that continually updates
the dependency without a stable API.

\" \*\*\* \" webOS OSE provides this different version.

This document only captures the version at the first release of a ROS
distribution and will not be updated as the dependencies move forward.
These versions are thus a low watermark.

Package manager use for dependencies:

- Ubuntu, Debian: apt, pip
- Windows: Chocolatey, pip
- macOS: Homebrew, pip
- RHEL: dnf
- OpenEmbedded: opkg

Build System Support:

- ament_cmake
- cmake
- setuptools

Kilted Kaiju (May 2025 - November 2026)
---------------------------------------

Targeted platforms:

+--------------+-----------------+------------+-----------------+---------+----------+--------------+
| Architecture | Ubuntu Noble    | Windows 10 | RHEL 9          | > macOS | Debian   | OpenEmbedded |
|              | (24.04)         | (VS2019)   |                 |         | Bookworm | / Yocto      |
|              |                 |            |                 |         | (12)     | Project      |
+==============+=================+============+=================+=========+==========+==============+
| > amd64      | Tier 1          | Tier 1     | Tier 2          | > Tier  | > Tier 3 | > Tier 3     |
|              | \[d\]\[a\]\[s\] | \[a\]\[s\] | \[d\]\[a\]\[s\] | > 3     | > \[s\]  | > \[s\]      |
|              |                 |            |                 | > \[s\] |          |              |
+--------------+-----------------+------------+-----------------+---------+----------+--------------+
| > arm64      | Tier 1          |            |                 |         | > Tier 3 | > Tier 3     |
|              | \[d\]\[a\]\[s\] |            |                 |         | > \[s\]  | > \[s\]      |
+--------------+-----------------+------------+-----------------+---------+----------+--------------+
| > arm32      | > Tier 3 \[s\]  |            |                 |         | > Tier 3 | > Tier 3     |
|              |                 |            |                 |         | > \[s\]  | > \[s\]      |
+--------------+-----------------+------------+-----------------+---------+----------+--------------+

The following indicators show what delivery mechanisms are available for
each platform.

\" \[d\] \" Distribution-specific (Debian, RPM, etc.) packages will be
provided for this platform for packages submitted to the rosdistro.

\" \[a\] \" Binary releases are provided as a single archive per
platform containing all packages in the Jazzy ROS 2 repos file[^14].

\" \[s\] \" Compilation from source.

Middleware Implementation Support:

  --------------------------------------------------------------------------------------
  Middleware Library         Middleware      Support   Platforms       Architectures
                             Provider        Level                     
  -------------------------- --------------- --------- --------------- -----------------
  rmw_fastrtps_cpp\*         eProsima        Tier 1    All Platforms   All Architectures
                             Fast-DDS                                  

  rmw_connextdds             RTI Connext     Tier 1    Ubuntu,         All Architectures
                                                       Windows, and    except arm64
                                                       macOS           

  rmw_cyclonedds_cpp         Eclipse Cyclone Tier 1    All Platforms   All Architectures
                             DDS                                       

  rmw_zenoh_cpp              Eclipse Zenoh   Tier 1    All Platforms   All Architectures

  rmw_fastrtps_dynamic_cpp   eProsima        Tier 2    All Platforms   All Architectures
                             Fast-DDS                                  

  rmw_gurumdds_cpp           GurumNetworks   Tier 3    Ubuntu and      All Architectures
                             GurumDDS                  Windows         except arm32
  --------------------------------------------------------------------------------------

\" \* \" means default RMW implementation.

Middleware implementation support is dependent upon the platform support
tier. For example a Tier 1 middleware implementation on a Tier 2
platform can only receive Tier 2 support.

Minimum language requirements:

- C++17
- Python 3.9

Dependency Requirements:

+--------------+-----------------------------+-----------------------------------------------------------------+
|              | > Required Support          | > Recommended Support                                           |
+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| Package      | > Ubuntu     | > Windows    | > RHEL 9     | > macOS\*\*  | Debian       | > OpenEmbedded\*\* |
|              | > Noble      | > 10\*\*     |              |              | Bookworm     |                    |
+==============+==============+==============+==============+==============+==============+====================+
| CMake        | > 3.28.3     | > 3.28.3     | > 3.26.5     | > 3.31.1     | > 3.25.1     | > 3.22.3           |
+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| EmPY         | > 3.3.4      | > 3.3.4      | > 3.3.4a     | > 3.3.4                                          |
+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| Gazebo       | > Ionic\*    | > N/A        | > N/A        | > Ionic\*    | > Ionic\*    | > N/A              |
+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| NumPy        | > 1.26.4     | > 1.26.4     | > 1.20.1     | > 2.1.3      | > 1.24.2     | > N/A              |
+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| Ogre         | > 1.12.10                                                                | > N/A              |
+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| OpenCV       | > 4.6.0      | > 4.9.0      | > 4.6.0      | > 4.10.0     | > 4.6.0      | > 4.1.0 /          |
|              |              |              |              |              |              | > 3.2.0\*\*\*      |
+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| OpenSSL      | > 3.0.13     | > 3.3.2      | > 3.2.2      | > 1.1.1w     | > 3.0.15     | 1.1.1d /           |
|              |              |              |              |              |              | 1.1.1b\*\*\*       |
+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| Python       | > 3.12.3     | > 3.12.3     | > 3.9.19     | > 3.13.0     | > 3.11.2     | > 3.8.2 /          |
|              |              |              |              |              |              | > 3.7.5\*\*\*      |
+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| Qt           | > 5.15.13    | > 5.15.8     | > 5.15.9     | > 5.15.16    | > 5.15.8     | 5.14.1 /           |
|              |              |              |              |              |              | 5.12.5\*\*\*       |
+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
|                             | > **Linux only**                                                               |
+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| PCL          | > 1.14.0     | > N/A        | > 1.12.0     | > 1.14.1     | > 1.13.0     | > 1.10.0           |
+--------------+--------------+--------------+--------------+--------------+--------------+--------------------+
| > **RMW Middleware**                                                                                         |
+--------------+-----------------------------------------------------------+-----------------------------------+
| Connext DDS  | > 7.3.0.0                                                 | > N/A                             |
+--------------+-----------------------------------------------------------+-----------------------------------+
| Cyclone DDS  | > 0.10.5                                                                                      |
+--------------+-----------------------------------------------------------------------------------------------+
| Fast-DDS     | > 2.14.4                                                                                      |
+--------------+-----------------------------+-----------------------------------------------------------------+
| Gurum DDS    | > 4.2.0                     | > N/A                                                           |
+--------------+-----------------------------+-----------------------------------------------------------------+
| Zenoh        | > 1.0.4                                                                                       |
+--------------+-----------------------------------------------------------------------------------------------+

\" \* \" means that this is not the upstream version (available on the
official Operating System repositories) but a package distributed by
OSRF or the community (package built and distributed on custom
repositories).

\" \*\* \" means that the dependency may see multiple version changes,
because the dependency uses a package manager that continually updates
the dependency without a stable API.

\" \*\*\* \" webOS OSE provides this different version.

This document only captures the version at the first release of a ROS
distribution and will not be updated as the dependencies move forward.
These versions are thus a low watermark.

Package manager use for dependencies:

- Ubuntu, Debian: apt, pip
- Windows: pixi/conda, pip
- macOS: Homebrew, pip
- RHEL: dnf
- OpenEmbedded: opkg

Build System Support:

- ament_cmake
- cargo
- cmake
- setuptools

Rolling Ridley (June 2020 - Ongoing)
------------------------------------

Rolling Ridley is a rolling development distribution of ROS 2 as
described in REP-2002[^15].

The target platform for Rolling Ridley will update as new upstream
distributions are selected for ROS 2 development. As of May 2025,
Rolling Ridley targets the same platforms as ROS 2 Kilted Kaiju.

Motivation
==========

This document is provided to help plan future development for libraries.
The primary platforms for ROS 2 are Canonical\'s Ubuntu releases, and
our intent is to track these releases as best as possible while also
allowing for current, thirdparty libraries to be used. macOS and Windows
being rolling distributions, ROS 2 will target the latest state of these
distributions at the time of the release.

Rationale
=========

Target platforms for future releases are speculative and are based on
consulting Ubuntu\'s release and end-of-life schedule[^16].

Copyright
=========

This document has been placed in the public domain.

[^1]: REP 2001 (<http://www.ros.org/reps/rep-2001.html>)

[^2]: C11 is required, but support for some non-compliant systems is
    also provided, e.g. MSVC.

[^3]: C11 is required, but support for some non-compliant systems is
    also provided, e.g. MSVC.

[^4]: Crystal ROS 2 Repos File
    (<https://github.com/ros2/ros2/blob/crystal/ros2.repos>)

[^5]: C11 is required, but support for some non-compliant systems is
    also provided, e.g. MSVC.

[^6]: Dashing ROS 2 Repos File
    (<https://github.com/ros2/ros2/blob/dashing/ros2.repos>)

[^7]: Eloquent ROS 2 Repos File
    (<https://github.com/ros2/ros2/blob/eloquent/ros2.repos>)

[^8]: Connext DDS 6.0.0 Support
    (<https://github.com/ros2/rmw_connext/issues/375>)

[^9]: Foxy ROS 2 Repos File
    (<https://github.com/ros2/ros2/blob/foxy/ros2.repos>)

[^10]: Galactic ROS 2 Repos File
    (<https://github.com/ros2/ros2/blob/galactic/ros2.repos>)

[^11]: Humble ROS 2 Repos File
    (<https://github.com/ros2/ros2/blob/humble/ros2.repos>)

[^12]: Iron ROS 2 Repos File
    (<https://github.com/ros2/ros2/blob/iron/ros2.repos>)

[^13]: Jazzy ROS 2 Repos File
    (<https://github.com/ros2/ros2/blob/jazzy/ros2.repos>)

[^14]: Kilted ROS 2 Repos File
    (<https://github.com/ros2/ros2/blob/rolling/ros2.repos>)

[^15]: REP 2002 (<http://www.ros.org/reps/rep-2002.html>)

[^16]: Ubuntu Releases with End-of-Life Dates
    (<https://wiki.ubuntu.com/Releases>)
