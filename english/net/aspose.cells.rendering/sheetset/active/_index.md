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
public static void SheetSet_Property_Active()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(456);

            // Create a PdfSaveOptions object
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Set the SheetSet property to include only the active sheet
            pdfSaveOptions.SheetSet = SheetSet.Active;

            // Save the workbook to a PDF file
            workbook.Save("SheetSetExample_ActiveSheet.pdf", pdfSaveOptions);

            // Set the SheetSet property to include all visible sheets
            pdfSaveOptions.SheetSet = SheetSet.Visible;

            // Save the workbook to a PDF file
            workbook.Save("SheetSetExample_VisibleSheets.pdf", pdfSaveOptions);

            // Set the SheetSet property to include all sheets
            pdfSaveOptions.SheetSet = SheetSet.All;

            // Save the workbook to a PDF file
            workbook.Save("SheetSetExample_AllSheets.pdf", pdfSaveOptions);

            return;
        }
```

### See Also

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


