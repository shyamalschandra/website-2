---
title: webOS OSE 1.2.0 Release
date: 2018-08-30
slug: webos-ose-1-2-0-release
posttype: release
toc: false
---

Key highlights of this release are as follows.

* [Bluetooth support](#bluetooth-support)
* [AI assistant service](#ai-assistant-service)
* [ROS bridge](#ros-bridge)
* [IoTivity sampler](#iotivity-sampler)

For a complete listing of changes, refer to the [release notes]({{< relref "webos-ose-1-2-0-release-notes" >}}).

## Bluetooth support

From this release, webOS OSE provides Bluetooth functionality with the implementation based on BlueZ v5.48.

The supported Bluetooth profiles and features of each profile are listed below:

* **Generic Access Profile (GAP)**
    * Query the status information of Bluetooth adapters
    * Start or cancel discovery of devices
    * Perform pairing and unpairing between a device and an adapter
* **Generic Attribute Profile (GATT)**
    * Discover services and get supported services
    * Read and write characteristic values
    * Read and write descriptor values
    * Monitor characteristics
    * Add and remove services
* **Serial Port Profile (SPP)**
    * Read and write data through the connection set up by virtual serial ports

## AI assistant service

AI assistant service is a native service that provides AI features for applications and services. All applications and services in webOS OSE can subscribe an AI response and perform various user scenarios by using the response.

You can start or stop AI assistant service using LS2 API. Currently, the AI assistant service supports speech recognition from Google Assistant.

AI assistant service enables you to develop applications and services that offer the following features.

* Activate a device using a wake-word such as *OK Google*, *Jane Doe* or any customized keyword
* Get information like the weather, time, and news using speech commands
* Control a device using speech commands

## ROS bridge

ROS 2.0 (ROS2) is a set of software libraries and tools that help to build robot-related applications. ROS2 makes it easy to communicate with multiple devices. With ROS bridge in webOS OSE, the topics published by web applications on webOS OSE can be shown on any type of ROS2 supported devices.

**Note:** For the detailed design concept of ROS2, refer to [ROS 2.0 Design](http://design.ros2.org/).

ROS bridge provides you with the following features so that you can develop robot-related applications more easily.

* Monitor connected ROS2 devices via ROS commands
* Run ros2 packages
* Subscribe or publish ros2 topics using LS2 API
* Call ros2 services using LS2 API

## IoTivity sampler

IoTivity sampler is an application that showcases the [OCF](http://openconnectivity.org/) functionality built into the webOS OSE.

IoTivity sampler runs on the IoT framework of webOS OSE using iotivity-node and IoTivity as the backend. Regarding the IoT framework of webOS OSE, refer to [IoT Connectivity in webOS OSE]({{< relref "2018-06-21-iot-connectivity" >}}).

For more information on how to run the IoTivity sampler, see [webOS Sample Apps](https://wiki.iotivity.org/webos#webos_sample_apps) in IoTivity Wiki.
