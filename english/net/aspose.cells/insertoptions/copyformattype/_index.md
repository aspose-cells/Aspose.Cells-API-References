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
public static void Property_CopyFormatType()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fill some data in the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Header1&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;Data1&quot;);
            worksheet.Cells[&quot;A3&quot;].PutValue(&quot;Data2&quot;);

            // Create InsertOptions and set CopyFormatType
            InsertOptions insertOptions = new InsertOptions();
            insertOptions.CopyFormatType = CopyFormatType.SameAsAbove;

            // Insert a row at the second position with the specified format type
            worksheet.Cells.InsertRows(1, 1, insertOptions);

            // Save the workbook
            workbook.Save(&quot;CopyFormatTypeExample.xlsx&quot;);
            workbook.Save(&quot;CopyFormatTypeExample.pdf&quot;);
            return;
        }
```

### See Also

* enum [CopyFormatType](../../copyformattype/)
* class [InsertOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


