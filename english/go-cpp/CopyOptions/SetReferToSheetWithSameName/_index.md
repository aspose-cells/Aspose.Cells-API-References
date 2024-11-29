---
title: SetReferToSheetWithSameName Method 
linktitle: SetReferToSheetWithSameName
second_title: Aspose.Cells for Go API Reference
description: 'SetReferToSheetWithSameName method. Encapsulates the function that represents setrefertosheetwithsamename in Go.'
type: docs
weight: 200
url: /go/copyoptions/setrefertosheetwithsamename/
---

## SetReferToSheetWithSameName function

In ms excel, when copying formulas which refer to other worksheets while copying a worksheet to another one,the copied formulas should refer to source workbook.However, for some situations user may need the copied formulas refer to worksheets with the same namein the same workbook, such as when those worksheets have been copied before this copy operation,then this property should be kept as true.

```go

func (instance *CopyOptions) SetReferToSheetWithSameName(value bool)  error

```

## Remarks


## See Also

* Class [CopyOptions](../)
* Namespace [Aspose.Cells](../../)
* Library [Aspose.Cells for Go](../../../)
