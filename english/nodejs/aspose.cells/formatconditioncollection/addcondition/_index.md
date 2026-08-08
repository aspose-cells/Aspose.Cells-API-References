---
title: "FormatConditionCollection.addCondition"
linktitle: "addCondition"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Adds a formatting condition."
type: docs
weight: 30
url: /nodejs/aspose.cells/formatconditioncollection/addcondition/
---

## addCondition(type, operatorType, formula1, formula2)

Adds a formatting condition.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | FormatConditionType |
| operatorType | Number | OperatorType |
| formula1 | String | The value or expression associated with conditional formatting. If the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "="=..."". |
| formula2 | String | The value or expression associated with conditional formatting. The input format is same with formula1 |

**Returns:** Number — `Number` Formatting condition object index;
