---
title: VbaProject.IsValidSigned
second_title: Aspose.Cells for .NET API Reference
description: VbaProject property. Indicates whether the signature of VBA project is valid or not
type: docs
url: /net/aspose.cells.vba/vbaproject/isvalidsigned/
---
## VbaProject.IsValidSigned property

Indicates whether the signature of VBA project is valid or not.

```csharp
public bool IsValidSigned { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(wb.VbaProject.IsValidSigned);
public void VbaProject_Property_IsValidSigned()
{
    Workbook wb = new Workbook(vbaDir + "example.xlsm");
    Assert.IsTrue(wb.VbaProject.IsSigned);
    Assert.IsTrue(wb.VbaProject.IsValidSigned);

    MemoryStream ms = new MemoryStream();
    wb.Save(ms, SaveFormat.Excel97To2003);

    Workbook validateWb = new Workbook(ms);
    Assert.IsTrue(validateWb.VbaProject.IsSigned);
    Assert.IsTrue(validateWb.VbaProject.IsValidSigned);
}
```

### See Also

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


