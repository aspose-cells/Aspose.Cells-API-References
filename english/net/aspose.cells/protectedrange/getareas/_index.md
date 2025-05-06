---
title: ProtectedRange.GetAreas
second_title: Aspose.Cells for .NET API Reference
description: ProtectedRange method. Gets all referred areas
type: docs
url: /net/aspose.cells/protectedrange/getareas/
---
## ProtectedRange.GetAreas method

Gets all referred areas.

```csharp
public CellArea[] GetAreas()
```

### Return Value

Returns all referred areas.

### Examples

```csharp
// Called: Assert.AreEqual(1, r.GetAreas().Length);
[Test]
         public void Method_GetAreas()
         {
           
             Workbook workbook = new Workbook();
             ProtectedRangeCollection pranges = workbook.Worksheets[0].AllowEditRanges;
             int index = pranges.Add(&quot;Range1&quot;, 0, 0, 10, 10);
             ProtectedRange r = pranges[index];
            Assert.AreEqual(1, r.GetAreas().Length);
             string x = &quot;O:WDG:WDD:(D;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1000)(A;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1013)&quot;;
             r.SecurityDescriptor = x;
             workbook.Save(Constants.destPath + &quot;CELLSNET41052.xlsx&quot;);
             workbook = new Workbook(Constants.destPath + &quot;CELLSNET41052.xlsx&quot;);
             Assert.AreEqual(workbook.Worksheets[0].AllowEditRanges[0].SecurityDescriptor, x);
         }
```

### See Also

* struct [CellArea](../../cellarea/)
* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


