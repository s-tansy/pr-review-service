---
uid: learn.wwl.work-with-data-in-aml.knowledge-check
title: Knowledge check
description: Knowledge check
durationInMinutes: 2
---
## quiz title: 

## Multiple Choice
You have a reference to a Workspace named ws. Which code retrieves the default datastore for the workspace?
( ) default_ds = Datastore.get(ws, 'default') {{That is incorrect. To get the default datastore, use the get_default_datastore method of the Workspace.}}
( ) default_ds = ws.Datastores[0] {{That is incorrect. To get the default datastore, use the get_default_datastore method of the Workspace.}}
(x) default_ds = ws.get_default_datastore() {{That is correct. To get the default datastore, use the get_default_datastore method of the Workspace.}}

## Multiple Choice
A datastore contains a CSV file of structured data that you want to use as a Pandas dataframe. Which kind of object should you create to make it easy to do this?
( ) A datastore. {{That is incorrect. A tabular dataset provides the easiest way to consume structured data as a Pandas dataframe.}}
(x) A tabular dataset. {{That is correct. A tabular dataset provides the easiest way to consume structured data as a Pandas dataframe.}}
( ) A file dataset. {{That is incorrect. A tabular dataset provides the easiest way to consume structured data as a Pandas dataframe.}}

## Multiple Choice
You want a script to stream data directly from a file dataset. Which mode should you use?
(x) as_mount() {{That is correct. To stream data directly from its source, use as_mount mode.}}
( ) as_download() {{That is incorrect. To stream data directly from its source, use as_mount mode.}}
( ) as_upload() {{That is incorrect. To stream data directly from its source, use as_mount mode.}}