---
title: Class ProtectedRange
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.ProtectedRange class. A specified range to be allowed to edit when the sheet protection is ON
type: docs
url: /net/aspose.cells/protectedrange/
---
## ProtectedRange class

A specified range to be allowed to edit when the sheet protection is ON.

```csharp
public class ProtectedRange
```

## Properties

| Name | Description |
| --- | --- |
| [CellArea](../../aspose.cells/protectedrange/cellarea/) { get; } | Gets the [`CellArea`](./cellarea/) object represents the cell area to be protected. |
| [IsProtectedWithPassword](../../aspose.cells/protectedrange/isprotectedwithpassword/) { get; } | Indicates whether the worksheets is protected with password. |
| [Name](../../aspose.cells/protectedrange/name/) { get; set; } | Gets the Range title. This is used as a descriptor, not as a named range definition. |
| [Password](../../aspose.cells/protectedrange/password/) { get; set; } | Represents the password to protect the range. |
| [SecurityDescriptor](../../aspose.cells/protectedrange/securitydescriptor/) { get; set; } | The security descriptor defines user accounts who may edit this range without providing a password to access the range. |

## Methods

| Name | Description |
| --- | --- |
| [AddArea](../../aspose.cells/protectedrange/addarea/)(int, int, int, int) | Adds a referred area to this |
| [GetAreas](../../aspose.cells/protectedrange/getareas/)() | Gets all referred areas. |

### Examples

```csharp
// Called: ProtectedRange r = pranges[index];
public void Cells_Type_ProtectedRange()
{
           
    Workbook workbook = new Workbook();
    ProtectedRangeCollection pranges = workbook.Worksheets[0].AllowEditRanges;
    int index = pranges.Add("Range1", 0, 0, 10, 10);
    ProtectedRange r = pranges[index];
   Assert.AreEqual(1, r.GetAreas().Length);
    string x = "O:WDG:WDD:(D;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1000)(A;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1013)";
    r.SecurityDescriptor = x;
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    Assert.AreEqual(workbook.Worksheets[0].AllowEditRanges[0].SecurityDescriptor, x);
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


