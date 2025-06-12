---
title: PivotPageFields.PageFieldCount
second_title: Aspose.Cells for .NET API Reference
description: PivotPageFields property. Gets the number of page fields
type: docs
url: /net/aspose.cells.pivot/pivotpagefields/pagefieldcount/
---
## PivotPageFields.PageFieldCount property

Gets the number of page fields.

```csharp
public int PageFieldCount { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotPageFieldsPropertyPageFieldCountDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for pivot table
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Region";
            worksheet.Cells["C1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = "North";
            worksheet.Cells["C2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = "South";
            worksheet.Cells["C3"].Value = 2000;
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = "East";
            worksheet.Cells["C4"].Value = 3000;

            // Create a pivot table
            int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Add fields to pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Page, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Page, "Region");

            // Get the PivotPageFields
            PivotFieldCollection pageFields = pivotTable.PageFields;

            // Display the current PageFieldCount
            Console.WriteLine("Current PageFieldCount: " + pageFields.Count);

            // Note: PageFieldCount is read-only, so we can't set it directly
            // We can only modify it by adding/removing page fields

            // Add another page field (will increase PageFieldCount)
            pivotTable.AddFieldToArea(PivotFieldType.Page, "Sales");
            Console.WriteLine("After adding field, PageFieldCount: " + pageFields.Count);

            // Save the workbook
            workbook.Save("PivotPageFieldsPropertyPageFieldCountDemo.xlsx");
        }
    }
}
```

### See Also

* class [PivotPageFields](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


