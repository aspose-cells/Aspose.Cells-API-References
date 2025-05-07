---
title: Name.IsVisible
second_title: Aspose.Cells for .NET API Reference
description: Name property. Indicates whether the name is visible
type: docs
url: /net/aspose.cells/name/isvisible/
---
## Name.IsVisible property

Indicates whether the name is visible.

```csharp
public bool IsVisible { get; set; }
```

### Examples

```csharp
// Called: workbook.Worksheets.Names[0].IsVisible = false;
[Test]
        public void Property_IsVisible()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
           
            Aspose.Cells.Range range = cells.CreateRange("A1", "B2");
            range.Name = "TestNamedRange";
            workbook.Worksheets.Names[0].IsVisible = false;
            workbook.Save(Constants.destPath + "TestHiddenName.xls");
        }
```

### See Also

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


