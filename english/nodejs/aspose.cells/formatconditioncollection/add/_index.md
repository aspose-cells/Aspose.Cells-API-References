---
title: "FormatConditionCollection.add"
linktitle: "add"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Adds a formatting condition and effected cell rang to the FormatConditions The FormatConditions can contain up to three conditional formats."
type: docs
weight: 10
url: /nodejs/aspose.cells/formatconditioncollection/add/
---

## add(cellArea, type, operatorType, formula1, formula2)

Adds a formatting condition and effected cell rang to the FormatConditions The FormatConditions can contain up to three conditional formats. References to the other sheets are not allowed in the formulas of conditional formatting. OperatorType

| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | CellArea | Conditional formatted cell range. |
| type | Number | FormatConditionType |
| operatorType | Number | OperatorType |
| formula1 | String | The value or expression associated with conditional formatting. |
| formula2 | String | The value or expression associated with conditional formatting |

**Returns:** Array of Number — `Array of Number` [0]:Formatting condition object index;[1] Effected cell rang index.
