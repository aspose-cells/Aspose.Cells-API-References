---
title: Style.Font
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets a Font object
type: docs
url: /net/aspose.cells/style/font/
---
## Style.Font property

Gets a `Font` object.

```csharp
public Font Font { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.DefaultStyle.Font.Size, 8);
[Test]
        public void Property_Font()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "seanb.xls");
            Assert.AreEqual(workbook.DefaultStyle.Font.Size, 8);
        }
```

### See Also

* class [Font](../../font/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


