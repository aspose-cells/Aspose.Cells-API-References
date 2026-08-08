---
title: "CellsHelper.createSafeSheetName"
linktitle: "createSafeSheetName"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Checks given sheet name and create a valid one when needed."
type: docs
weight: 250
url: /nodejs/aspose.cells/cellshelper/createsafesheetname-1/
---

## createSafeSheetName(nameProposal, replaceChar) (static)

Checks given sheet name and create a valid one when needed. If given sheet name conforms to the rules of excel sheet name, then return it. Otherwise string will be truncated if length exceeds the limit and invalid characters will be replaced with given character, then return the rebuilt string value.

| Parameter | Type | Description |
| --- | --- | --- |
| nameProposal | String | sheet name to be used |
| replaceChar | char | character which will be used to replace invalid characters in given sheet name |

**Returns:** String — `String`
