---
title: Workbook.CellsDataTableFactory
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Gets the factory for building ICellsDataTable from custom objects
type: docs
url: /net/aspose.cells/workbook/cellsdatatablefactory/
---
## Workbook.CellsDataTableFactory property

Gets the factory for building ICellsDataTable from custom objects

```csharp
public CellsDataTableFactory CellsDataTableFactory { get; }
```

### Examples

```csharp
// Called: CellsDataTableFactory factory = workbook.CellsDataTableFactory;
public static void Workbook_Property_CellsDataTableFactory()
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

* class [CellsDataTableFactory](../../cellsdatatablefactory/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


