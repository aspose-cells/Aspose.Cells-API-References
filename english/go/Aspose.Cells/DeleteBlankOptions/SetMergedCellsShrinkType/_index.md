---
title: SetMergedCellsShrinkType Method 
linktitle: SetMergedCellsShrinkType
second_title: Aspose.Cells for Go API Reference
description: 'SetMergedCellsShrinkType method. Encapsulates the function that represents setmergedcellsshrinktype in Go.'
type: docs
weight: 200
url: /go/aspose.cells/deleteblankoptions/setmergedcellsshrinktype/
---

## SetMergedCellsShrinkType function

Indicates how to process merged cells when deleting blank rows/columns.<br></br>For <see cref="MergedCellsShrinkType.KeepHeaderOnly"/>, all cells in it will be taken as blank except the non-blank top-left cell. It is the default value of this property.<br></br>For <see cref="MergedCellsShrinkType.None"/>, all cells in it will be taken as non-blank.<br></br>For <see cref="MergedCellsShrinkType.ShrinkToFit"/>, all cells outside the content display area will be taken as blank.<br></br>

```go

func (instance *DeleteBlankOptions) SetMergedCellsShrinkType(value MergedCellsShrinkType)  error

```

## Remarks


## See Also

* Class [DeleteBlankOptions](../)
* Namespace [Aspose.Cells](../../)
* Library [Aspose.Cells for Go](../../../)
