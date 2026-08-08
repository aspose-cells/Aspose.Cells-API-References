---
title: "Workbook.startAccessCache"
linktitle: "startAccessCache"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Starts the session that uses caches to access data."
type: docs
weight: 910
url: /nodejs/aspose.cells/workbook/startaccesscache/
---

## startAccessCache(opts)

Starts the session that uses caches to access data. If the cache of specified data access requires some data models in worksheet to be "read-only", then corresponding data models in every worksheet in this workbook will be taken as "read-only" and user should not change any of them. After finishing the access to the data, closeAccessCache(int) should be invoked with same options to clear all caches and recover normal access mode.

| Parameter | Type | Description |
| --- | --- | --- |
| opts | Number | AccessCacheOptions |
