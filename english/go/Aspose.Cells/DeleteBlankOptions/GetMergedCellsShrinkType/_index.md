---
title: GetMergedCellsShrinkType Method 
linktitle: GetMergedCellsShrinkType
second_title: Aspose.Cells for Go API Reference
description: 'GetMergedCellsShrinkType method. Encapsulates the function that represents getmergedcellsshrinktype in Go.'
type: docs
weight: 200
url: /go/aspose.cells/deleteblankoptions/getmergedcellsshrinktype/
---

## GetMergedCellsShrinkType function

Indicates how to process merged cells when deleting blank rows/columns.<br></br>For <see cref="MergedCellsShrinkType.KeepHeaderOnly"/>, all cells in it will be taken as blank except the non-blank top-left cell. It is the default value of this property.<br></br>For <see cref="MergedCellsShrinkType.None"/>, all cells in it will be taken as non-blank.<br></br>For <see cref="MergedCellsShrinkType.ShrinkToFit"/>, all cells outside the content display area will be taken as blank.<br></br>

```go

func (instance *DeleteBlankOptions) GetMergedCellsShrinkType()  (MergedCellsShrinkType,  error) 

```

## Remarks


## See Also

* Class [DeleteBlankOptions](../)
* Namespace [Aspose.Cells](../../)
* Library [Aspose.Cells for Go](../../../)
