---
title: ProtectedRange.IsProtectedWithPassword
second_title: Aspose.Cells for .NET API Reference
description: ProtectedRange property. Indicates whether the worksheets is protected with password
type: docs
url: /net/aspose.cells/protectedrange/isprotectedwithpassword/
---
## ProtectedRange.IsProtectedWithPassword property

Indicates whether the worksheets is protected with password.

```csharp
public bool IsProtectedWithPassword { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(r.IsProtectedWithPassword);
public void ProtectedRange_Property_IsProtectedWithPassword()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    ProtectedRange r = workbook.Worksheets[0].AllowEditRanges[0];
    Assert.IsTrue(r.IsProtectedWithPassword);
    workbook.Save(Constants.destPath + "example.xlsx");

}
```

### See Also

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


