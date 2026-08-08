---
title: "Cells.merge"
linktitle: "merge"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Merges a specified range of cells into a single cell."
type: docs
weight: 1440
url: /nodejs/aspose.cells/cells/merge-2/
---

## merge(firstRow, firstColumn, totalRows, totalColumns, checkConflict, mergeConflict)

Merges a specified range of cells into a single cell. Reference the merged cell via the address of the upper-left cell in the range. If mergeConflict is true and the merged range conflicts with other merged cells, other merged cells will be automatically removed.

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Number | First row of this range(zero based) |
| firstColumn | Number | First column of this range(zero based) |
| totalRows | Number | Number of rows(one based) |
| totalColumns | Number | Number of columns(one based) |
| checkConflict | boolean | Indicates whether check the merged cells intersects other merged cells |
| mergeConflict | boolean | Merge conflict merged ranges. |
