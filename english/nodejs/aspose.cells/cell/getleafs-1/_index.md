---
title: "Cell.getLeafs"
linktitle: "getLeafs"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Get all cells which will be updated when this cell is modified."
type: docs
weight: 330
url: /nodejs/aspose.cells/cell/getleafs-1/
---

## getLeafs(recursive)

Get all cells which will be updated when this cell is modified. NOTE: This class is now obsolete. Instead, please use Cell.GetDependentsInCalculation(bool) to get all dependents in calculation chain. This property will be removed 12 months later since May 2022. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| recursive | boolean | Whether returns those leafs that do not reference to this cell directly but reference to other leafs of this cell |

**Returns:** Iterator — `Iterator` Enumerator to enumerate all dependents(Cell)
