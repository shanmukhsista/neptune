---
sidebar_position: 1
---

## Definition

Analytics schemas can be defined by a user for their tenant. The general idea of Neptune is to provide fast query 
access to any arbitrary data elements. 


## Validation

Optional schema validation can be performed for each field. 

# Disk Storage

A schema is a collection of Records. Each of these records will be stored on Disk with some 'locality' in mind.

While a new file may be created for each column, we must ensure that the number of files is not very high on disk. 

Each disk file must have a max size, after which a new file will be created.

# File Storage Design

