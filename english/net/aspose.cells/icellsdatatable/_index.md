---
title: Interface ICellsDataTable
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.ICellsDataTable interface. Represents data table
type: docs
url: /net/aspose.cells/icellsdatatable/
---
## ICellsDataTable interface

Represents data table.

```csharp
public interface ICellsDataTable
```

## Properties

| Name | Description |
| --- | --- |
| [Columns](../../aspose.cells/icellsdatatable/columns/) { get; } | Gets the columns' name. |
| [Count](../../aspose.cells/icellsdatatable/count/) { get; } | Gets the count of the records. -1 for unknown records count. |
| [Item](../../aspose.cells/icellsdatatable/item/) { get; } | Gets the data stored in the column specified by index. (2 indexers) |

## Methods

| Name | Description |
| --- | --- |
| [BeforeFirst](../../aspose.cells/icellsdatatable/beforefirst/)() | Move the cursor to the front of this object, just before the first row. |
| [Next](../../aspose.cells/icellsdatatable/next/)() | Moves the cursor down one row from its current position. |

### Examples

```csharp
// Called: ICellsDataTable dataTable = factory.GetInstance(dataList);
public static void Type_ICellsDataTable()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some sample data
            List<CustomData> dataList = new List<CustomData>
            {
                new CustomData { Id = 1, Name = "John Doe", Age = 30 },
                new CustomData { Id = 2, Name = "Jane Smith", Age = 25 },
                new CustomData { Id = 3, Name = "Sam Brown", Age = 35 }
            };

            // Get the CellsDataTableFactory instance from the workbook
            CellsDataTableFactory factory = workbook.CellsDataTableFactory;

            // Create an ICellsDataTable instance from the custom data list
            ICellsDataTable dataTable = factory.GetInstance(dataList);

            // Import the data table into the worksheet starting at cell A1
            sheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

            // Save the workbook
            workbook.Save("CellsDataTableFactoryDemo.xlsx");
            workbook.Save("CellsDataTableFactoryDemo.pdf");
        }
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


