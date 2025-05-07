---
title: Font.Name
second_title: Aspose.Cells for .NET API Reference
description: Font property. Gets or sets the name of the Font
type: docs
url: /net/aspose.cells/font/name/
---
## Font.Name property

Gets or sets the name of the [`Font`](../).

```csharp
public virtual string Name { get; set; }
```

### Examples

```csharp
// Called: font.Name = "0123456789012345678901234567890123456789";
[Test, ExpectedException(typeof(CellsException))]
#endif
        public void Property_Name()
        {
            Workbook workbook = new Workbook();
            Aspose.Cells.Font font = workbook.DefaultStyle.Font;
            font.Name = "0123456789012345678901234567890123456789";
        }
```

### See Also

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


