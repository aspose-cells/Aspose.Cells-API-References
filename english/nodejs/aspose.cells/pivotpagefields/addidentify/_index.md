---
title: "PivotPageFields.addIdentify"
linktitle: "addIdentify"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Sets which item label in each page field to use to identify the data range."
type: docs
weight: 20
url: /nodejs/aspose.cells/pivotpagefields/addidentify/
---

## addIdentify(rangeIndex, pageItemIndex)

Sets which item label in each page field to use to identify the data range. The pageItemIndex.Length must be equal to PageFieldCount, so please add the page field first.

| Parameter | Type | Description |
| --- | --- | --- |
| rangeIndex | Number | The consolidation data range index. |
| pageItemIndex | Array of Number | The page item index in the each page field. pageItemIndex[2] = 1 means the second item in the third field to use to identify this range. pageItemIndex[1] = -1 means no item in the second field to use to identify this range and MS will auto create "blank" item in the second field to identify this range. |
