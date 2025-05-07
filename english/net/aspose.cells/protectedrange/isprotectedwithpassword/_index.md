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
[Test]
        public void Property_IsProtectedWithPassword()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet51922.xlsx");
            ProtectedRange r = workbook.Worksheets[0].AllowEditRanges[0];
            Assert.IsTrue(r.IsProtectedWithPassword);
            workbook.Save(Constants.destPath + "CellsNet51922.xlsb");
            workbook = new Workbook(Constants.destPath + "CellsNet51922.xlsb");
            Assert.IsTrue(r.IsProtectedWithPassword);

        }
```

### See Also

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


