---
title: SheetSet.Active
second_title: Aspose.Cells for .NET API Reference
description: SheetSet property. Gets a set with active sheet of the workbook
type: docs
url: /net/aspose.cells.rendering/sheetset/active/
---
## SheetSet.Active property

Gets a set with active sheet of the workbook.

```csharp
public static SheetSet Active { get; }
```

### Examples

```csharp
// Called: pdfSaveOptions.SheetSet = SheetSet.Active;
public static void Property_Active()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Sample Data&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(123);
            worksheet.Cells[&quot;A3&quot;].PutValue(456);

            // Create a PdfSaveOptions object
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Set the SheetSet property to include only the active sheet
            pdfSaveOptions.SheetSet = SheetSet.Active;

            // Save the workbook to a PDF file
            workbook.Save(&quot;SheetSetExample_ActiveSheet.pdf&quot;, pdfSaveOptions);

            // Set the SheetSet property to include all visible sheets
            pdfSaveOptions.SheetSet = SheetSet.Visible;

            // Save the workbook to a PDF file
            workbook.Save(&quot;SheetSetExample_VisibleSheets.pdf&quot;, pdfSaveOptions);

            // Set the SheetSet property to include all sheets
            pdfSaveOptions.SheetSet = SheetSet.All;

            // Save the workbook to a PDF file
            workbook.Save(&quot;SheetSetExample_AllSheets.pdf&quot;, pdfSaveOptions);

            return;
        }
```

### See Also

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


