---
title: ProtectedRange.SecurityDescriptor
second_title: Aspose.Cells for .NET API Reference
description: ProtectedRange property. The security descriptor defines user accounts who may edit this range without providing a password to access the range
type: docs
url: /net/aspose.cells/protectedrange/securitydescriptor/
---
## ProtectedRange.SecurityDescriptor property

The security descriptor defines user accounts who may edit this range without providing a password to access the range.

```csharp
public string SecurityDescriptor { get; set; }
```

### Examples

```csharp
// Called: r.SecurityDescriptor = x;
[Test]
         public void Property_SecurityDescriptor()
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

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


