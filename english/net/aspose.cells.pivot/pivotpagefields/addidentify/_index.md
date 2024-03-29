---
title: PivotPageFields.AddIdentify
second_title: Aspose.Cells for .NET API Reference
description: PivotPageFields method. Sets which item label in each page field to use to identify the data range. The pageItemIndex.Length must be equal to PageFieldCount so please add the page field first
type: docs
url: /net/aspose.cells.pivot/pivotpagefields/addidentify/
---
## PivotPageFields.AddIdentify method

Sets which item label in each page field to use to identify the data range. The pageItemIndex.Length must be equal to PageFieldCount, so please add the page field first.

```csharp
public void AddIdentify(int rangeIndex, int[] pageItemIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rangeIndex | Int32 | The consolidation data range index. |
| pageItemIndex | Int32[] | The page item index in the each page field. pageItemIndex[2] = 1 means the second item in the third field to use to identify this range. pageItemIndex[1] = -1 means no item in the second field to use to identify this range and MS will auto create "blank" item in the second field to identify this range. |

### See Also

* class [PivotPageFields](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


