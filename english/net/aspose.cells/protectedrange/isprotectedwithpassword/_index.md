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
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet51922.xlsx&quot;);
            ProtectedRange r = workbook.Worksheets[0].AllowEditRanges[0];
            Assert.IsTrue(r.IsProtectedWithPassword);
            workbook.Save(Constants.destPath + &quot;CellsNet51922.xlsx&quot;);

        }
```

### See Also

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


