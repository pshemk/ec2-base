# Overview

This repo contains a single role that sets up an EC2 instance.

## Usage

The easiest way is just to clone the whole repository and than copy the _ec2-base_ role into your own work.

## Parameters

Parameters are passed via *Tags* on resources:

| Resource type | Tag | Used for | default |
|---|---|---|---|
| AWS::EC2::Instance | Name | hostname | |
| AWS::EC2::Volume | Mount | volume mount point | data |
| AWS::EC2::Volume |Fs_type | filesystem to use | xfs |

