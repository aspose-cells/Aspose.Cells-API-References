---
title: PivotTableCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: PivotTableCollection property. Gets the PivotTable report by index
type: docs
url: /net/aspose.cells.pivot/pivottablecollection/item/
---
## PivotTableCollection indexer (1 of 3)

Gets the PivotTable report by index.

```csharp
public PivotTable this[int index] { get; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Create a workbook from source file
            Workbook workbook = new Workbook("example.xlsx");
            
            // Access first worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Access pivot tables collection
            PivotTableCollection pivotTables = worksheet.PivotTables;
            
            // Access first pivot table using Item property (indexer)
            PivotTable pivotTable = pivotTables[0];
            
            // Calculate pivot table data
            pivotTable.CalculateData();
            
            // Save the modified workbook
            workbook.Save("output.xlsx");
        }
    }
}
```

### See Also

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## PivotTableCollection indexer (2 of 3)

Gets the PivotTable report by pivottable's name.

```csharp
public PivotTable this[string name] { get; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Create sample data
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B4"].PutValue(3000);

            // Add a pivot table
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Configure pivot table using Item property
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Refresh and calculate data
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Access pivot table using Item property
            PivotTable tableFromCollection = sheet.PivotTables["PivotTable1"];
            Console.WriteLine("Pivot table data source: " + string.Join(", ", tableFromCollection.DataSource));

            // Modify data and refresh
            sheet.Cells["B2"].PutValue(1500);
            tableFromCollection.RefreshData();
            Console.WriteLine("Updated pivot table values");

            // Save the workbook
            workbook.Save("PivotTableDemo.xlsx");
        }
    }
}
```

### See Also

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## PivotTableCollection indexer (3 of 3)

Gets the PivotTable report by pivottable's position.

```csharp
public PivotTable this[int row, int column] { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionPropertyItemDemo2
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for the pivot table
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["B4"].Value = 8;

            // Add a pivot table
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Access pivot tables using Item property (by index)
            Console.WriteLine("First pivot table name: " + pivotTables[0].Name);

            // Add another pivot table
            index = pivotTables.Add("A1:B4", "E10", "PivotTable2");
            
            // Access pivot tables using Item property (by name)
            Console.WriteLine("Second pivot table name: " + pivotTables["PivotTable2"].Name);

            // Modify the second pivot table through Item property
            pivotTables["PivotTable2"].RefreshData();
            pivotTables["PivotTable2"].CalculateData();

            // Save the result
            workbook.Save("PivotTableCollectionItemDemo.xlsx");
        }
    }
}
```

### See Also

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


