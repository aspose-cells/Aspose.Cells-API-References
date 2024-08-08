﻿---
title: MergedCellsShrinkType
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the strategy to shrink merged cells for operations such as deleting blank rowscolumn.
type: docs
url: /nodejs-cpp/mergedcellsshrinktype/
---

## MergedCellsShrinkType enumeration
Represents the strategy to shrink merged cells for operations such as deleting blank rows/column.
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` | Leaves the merged cells as it is without any modification. |
| ShrinkToFit | `1` | Shrinks the merged area if needed, by removing rows from the bottom or columns from the right, while ensuring all content remains visible. |
| KeepHeaderOnly | `2` | Only keeps the header rows/columns of the merged area if needed. |

