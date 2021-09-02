# Overview

This repo contains a single role that sets up an EC2 instance.

## Usage

The easiest way is just to clone the whole repository and than copy the _ec2-base_ role into your own work.

## Parameters

Parameters are passed via *Tags* on resources:

| Resource type | Tag | Used for | default |
|---|---|---|---|
| AWS::EC2::Instance | Name | hostname | |
| AWS::EC2::Volume | Name | volume mount point | data |
| AWS::EC2::Volume | Device | device name (legacy hypervisor) |  |
| AWS::EC2::Volume |Fs_type | filesystem to use | xfs |

if the Name inside the Volume tag is set to 'swap' the disk is used for swap.