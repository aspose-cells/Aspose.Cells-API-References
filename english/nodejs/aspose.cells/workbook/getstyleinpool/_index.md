---
title: "Workbook.getStyleInPool"
linktitle: "getStyleInPool"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Gets the style in the style pool."
type: docs
weight: 470
url: /nodejs/aspose.cells/workbook/getstyleinpool/
---

## getStyleInPool(index)

Gets the style in the style pool. All styles in the workbook will be gathered into a pool. There is only a simple reference index in the cells. If the returned style is changed, the style of all cells(which refers to this style) will be changed.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The index. |

**Returns:** Style — `Style` The style in the pool corresponds to given index, may be null.
