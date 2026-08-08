---
title: "WorksheetCollection.registerAddInFunction"
linktitle: "registerAddInFunction"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Adds addin function into the workbook"
type: docs
weight: 460
url: /nodejs/aspose.cells/worksheetcollection/registeraddinfunction/
---

## registerAddInFunction(addInFile, functionName, lib)

Adds addin function into the workbook

| Parameter | Type | Description |
| --- | --- | --- |
| addInFile | String | the file contains the addin functions |
| functionName | String | the addin function name |
| lib | boolean | whether the given addin file is in the directory or sub-directory of Workbook Add-In library. This flag takes effect and makes difference when given addInFile is of relative path: true denotes the path is relative to Add-In library and false denotes the path is relative to this Workbook. |

**Returns:** Number — `Number` ID of the data which contains given addin function
