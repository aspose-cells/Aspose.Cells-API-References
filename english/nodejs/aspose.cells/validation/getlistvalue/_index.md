---
title: "Validation.getListValue"
linktitle: "getListValue"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Get the value for list of the validation for the specified cell."
type: docs
weight: 190
url: /nodejs/aspose.cells/validation/getlistvalue/
---

## getListValue(row, column)

Get the value for list of the validation for the specified cell. Only for validation whose type is List and has been applied to given cell, otherwise null will be returned.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | The row index. |
| column | Number | The column index. |

**Returns:** Object — `Object` The value to produce the list of this validation for the specified cell. If the list references to a range, then the returned value will be a ReferredArea object; Otherwise the returned value may be null, object[], or simple object.
