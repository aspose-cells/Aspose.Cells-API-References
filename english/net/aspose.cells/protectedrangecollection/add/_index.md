---
title: ProtectedRangeCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: ProtectedRangeCollection method. Adds a ProtectedRange item to the collection
type: docs
url: /net/aspose.cells/protectedrangecollection/add/
---
## ProtectedRangeCollection.Add method

Adds a [`ProtectedRange`](../../protectedrange/) item to the collection.

```csharp
public int Add(string name, int startRow, int startColumn, int endRow, int endColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | Range title. This is used as a descriptor, not as a named range definition. |
| startRow | Int32 | Start row index of the range. |
| startColumn | Int32 | Start column index of the range. |
| endRow | Int32 | End row index of the range. |
| endColumn | Int32 | End column index of the range. |

### Return Value

object index.

### Examples

```csharp
// Called: int index = pranges.Add("Range1", 0, 0, 10, 10);
[Test]
         public void Method_Int32_()
         {
           
             Workbook workbook = new Workbook();
             ProtectedRangeCollection pranges = workbook.Worksheets[0].AllowEditRanges;
             int index = pranges.Add("Range1", 0, 0, 10, 10);
             ProtectedRange r = pranges[index];
            Assert.AreEqual(1, r.GetAreas().Length);
             string x = "O:WDG:WDD:(D;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1000)(A;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1013)";
             r.SecurityDescriptor = x;
             workbook.Save(Constants.destPath + "CELLSNET41052.xlsx");
             workbook = new Workbook(Constants.destPath + "CELLSNET41052.xlsx");
             Assert.AreEqual(workbook.Worksheets[0].AllowEditRanges[0].SecurityDescriptor, x);
         }
```

### See Also

* class [ProtectedRangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


