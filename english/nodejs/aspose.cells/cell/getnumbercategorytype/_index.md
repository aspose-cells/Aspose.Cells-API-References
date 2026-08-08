---
title: "Cell.getNumberCategoryType"
linktitle: "getNumberCategoryType"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents the category type of this cell's number formatting."
type: docs
weight: 360
url: /nodejs/aspose.cells/cell/getnumbercategorytype/
---

## getNumberCategoryType()

Represents the category type of this cell's number formatting. The value of the property is NumberCategoryType integer constant.When cell's formatting pattern is combined with conditional formatting patterns, then the returned type is corresponding to the part which is used for current value of this cell. For example, if the formatting pattern for this cell is "#,##0;(#,##0);"-";@", then when cell's value is numeric and not 0, the returned type is NumberCategoryType.NUMBER; When cell's value is 0 or not numeric value, the returned type is NumberCategoryType.TEXT.
