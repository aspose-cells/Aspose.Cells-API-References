---
title: Worksheet.ViewType
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets and sets the view type
type: docs
url: /net/aspose.cells/worksheet/viewtype/
---
## Worksheet.ViewType property

Gets and sets the view type.

```csharp
public ViewType ViewType { get; set; }
```

### Examples

```csharp
// Called: worksheet.ViewType = ViewType.PageBreakPreview;
public static void Property_ViewType()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Set the view type of the worksheet to PageBreakPreview
            worksheet.ViewType = ViewType.PageBreakPreview;
            
            // Save the workbook
            workbook.Save("ViewTypeExample.xlsx");

            return;
        }
```

### See Also

* enum [ViewType](../../viewtype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


