---
title: Worksheet.Shapes
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Returns all drawing shapes in this worksheet
type: docs
url: /net/aspose.cells/worksheet/shapes/
---
## Worksheet.Shapes property

Returns all drawing shapes in this worksheet.

```csharp
public ShapeCollection Shapes { get; }
```

### Examples

```csharp
// Called: sheet.Shapes[iShape].UpdateSelectedValue();
public void Worksheet_Property_Shapes()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsm");
    foreach (Worksheet sheet in workbook.Worksheets)
    {

        for (int iShape = 0; iShape < sheet.Shapes.Count; iShape++)
        {
            if (sheet.Shapes[iShape].Name.CompareTo("Signature_Valideur") == 0)
            {

                sheet.Shapes[iShape].UpdateSelectedValue();
            }
        }

        sheet.PageSetup.PaperSize = PaperSizeType.PaperA4;
    }
    workbook.Save(Constants.destPath + "example.pdf");
}
```

### See Also

* class [ShapeCollection](../../../aspose.cells.drawing/shapecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


