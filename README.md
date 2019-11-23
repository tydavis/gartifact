# gartifact

Golang artifact frontend for Java (Maven, Gradle), NPM, Docker, and Python

## Purpose

gartifact is a cloud-storage-backed, multi-master package repository host. It is
built with s3 or GCS as its only backing store. There is no persistent local
state, no local database, only files in the backing store.  This means gartifact
will continue scaling as long as the backing store contiues to take the
appropriate connection load. 

## Why not X instead

Why use gartifact instead of Nexus or Artifactory? 

- gartifact is a single binary
- gartifact uses a single configuration file
- gartifact has no database or system state
- gartifact is built to be highly concurrent 
- gartifact can be deployed on anything which is an available Go compiler target

