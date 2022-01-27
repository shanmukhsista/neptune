---
sidebar_position: 1
---

# Column

A column is a logical container to store a certain subset of data. A column can hold values for supported Data Types. 

## Layout

In memory, each key that is sent to our analytics data warehouse is modeled as a column within our store. 

# Disk Storage

Each column is stored as a separate file on disk. 

Updating a single column requires updating an entire set of columns. 


Solution 

only non null column values are updated. 

nulls are added to the rocksdb storage