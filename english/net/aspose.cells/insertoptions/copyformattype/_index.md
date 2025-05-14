---
title: InsertOptions.CopyFormatType
second_title: Aspose.Cells for .NET API Reference
description: InsertOptions property. 
type: docs
url: /net/aspose.cells/insertoptions/copyformattype/
---
## InsertOptions.CopyFormatType property

```csharp
public CopyFormatType CopyFormatType { get; set; }
```

### Examples

```csharp
// Called: insertOptions.CopyFormatType = CopyFormatType.SameAsAbove;
public static void InsertOptions_Property_CopyFormatType()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fill some data in the worksheet
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");

            // Create InsertOptions and set CopyFormatType
            InsertOptions insertOptions = new InsertOptions();
            insertOptions.CopyFormatType = CopyFormatType.SameAsAbove;

            // Insert a row at the second position with the specified format type
            worksheet.Cells.InsertRows(1, 1, insertOptions);

            // Save the workbook
            workbook.Save("CopyFormatTypeExample.xlsx");
            workbook.Save("CopyFormatTypeExample.pdf");
            return;
        }
```

### See Also

* enum [CopyFormatType](../../copyformattype/)
* class [InsertOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


