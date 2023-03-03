---
layout: page
title: Born-Digital Archives
parent: Ingest
---

## Package Requirements

A Born-Digital Archives package must conform to the folder and file structure shown in the General Born-Digital Archives Package.
An example package for the Finding Aid Component is also included on this page, as it is the most common Born-Digital Archives package type.

### General Born-Digital Archives Package

![alt text]({{site.baseurl}}/assets/img/DA_package_general.svg "Diagram showing the file and folder structure of a General 
Born-Digital Archives Package")

All Born-Digital Archives package conforms to this structure. The top-level folder, named "Finding Aid component", must have two 
folders, namely, a "metadata" folder and an "objects" folder. Within the metadata folder, it may have a "submissionDocumentation" folder.
Both the metadata and submissionDocumentation folders may or may not have any files. When there are files in the metadata folder, it could
include CSV files, Digital Forensics XML files, or any other types of metadata relevant to the object(s). In the "objects" folder, it may
have more files and folders structures, depending on what types of content it is, and its original arrangement.

### Example Package of Finding Aid Component from Forensic Toolkit

![alt text]({{site.baseurl}}/assets/img/DA_package_example_FA_Component_FTK.svg "Diagram showing the file and folder structure of an 
Example Package of Finding Aid Component from FTK")

This diagram shows how a package from the Finding Aid Component exported from FTK (Forensic Toolkit) may look like. The top-level folder should 
be named after the finding aid component ID, aka the Electronic Records Identifier, e.g. M1234_ER_0001. This top-level folder should also 
include a "metadata" and an "objects" folder. Within the "metadata" folder, there should be a CSV file, named with the same finding aid component
ID. Within the "objects" folder, it should have one or more files.

## Data Model

Born-Digital Archives Data Model is created to accommodate a wide range of content collected by the NYPL 
[Digital Archives program](https://nypl.github.io/digarch/). It is designed to be adaptable to legacy collections as well as Digital 
Archives' future acquisitions.

### Data Model Description

Born-Digital Archives content contains different types of components, including but not limited to finding aid (FA) components, disk images, 
and file transfers. This data model is created based on FA component packages, and describes how the package will be structured after ingested 
into Preservica.

Each component forms a Structural Object (SO), named as "DI/EM/ER Container", which can be understood as a folder. DI stands for Digital Image; 
EM stands for Email; and ER stands for Electronic Record. DI/EM/ER Container must have one metadata SO, named "(original folder title)_metadata",
 and one contents SO, "(original folder title)_contents". Within the metadata SO, there may not have any file, or it may have metadata file(s). 
 Within the contents SO, there can be Information Object(s) (IO), also known as asset(s), and/or file and folder hierarchy, depending on the original 
 content structure.

![alt text]({{site.baseurl}}/assets/img/svg_data_model_born_digital_archives.svg "Diagram using the Unified Modeling Language showing the Data Model of 
the Born-Digital Archives, including the data classification and its relationships, folder names, metadata fragments, security tags")

## Process

Coming soon.