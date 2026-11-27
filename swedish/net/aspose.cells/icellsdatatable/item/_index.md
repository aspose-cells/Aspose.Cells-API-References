---
title: "ICellsDataTable.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ICellsDataTable egenskap. Hämtar data som lagras i kolumnen som anges av index"
type: docs
url: /sv/net/aspose.cells/icellsdatatable/item/
---
## ICellsDataTable indexer (1 of 2)

Hämtar data som lagras i kolumnen som specificeras av index.

```csharp
public object this[int columnIndex] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| columnIndex | Det nollbaserade indexet för kolumnen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ICellsDataTablePropertyItemDemo
    {
        public static void Run()
        {
            // Skapa anpassad ICellsDataTable med exempeldata
            ICellsDataTable dataTable = new SampleDataTable();

            // Återställ markörens position
            dataTable.BeforeFirst();

            Console.WriteLine("Reading data using Item property:");
            while (dataTable.Next())
            {
                // Åtkomst till värden efter kolumnindex
                Console.WriteLine($"Product: {dataTable[0]}, Price: {dataTable[1]}, Stock: {dataTable[2]}");

                // Åtkomst till värden efter kolumnnamn
                Console.WriteLine($"Product: {dataTable["Product"]}, Price: {dataTable["Price"]}, Stock: {dataTable["Stock"]}\n");
            }
        }
    }

    internal class SampleDataTable : ICellsDataTable
    {
        private readonly string[] columns = { "Product", "Price", "Stock" };
        private readonly object[][] data = 
        {
            new object[] { "Laptop", 999.99, 15 },
            new object[] { "Phone", 699.99, 25 },
            new object[] { "Tablet", 299.99, 50 }
        };
        private int currentRow = -1;

        public string[] Columns => columns;
        public int Count => data.Length;

        public object this[int columnIndex] => data[currentRow][columnIndex];
        public object this[string columnName] => data[currentRow][Array.IndexOf(columns, columnName)];

        public void BeforeFirst() => currentRow = -1;
        public bool Next() => ++currentRow < data.Length;
    }
}
```

### Se även

* interface [ICellsDataTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ICellsDataTable indexer (2 of 2)

Hämtar data som lagras i kolumnen som anges med kolumnnamn.

```csharp
public object this[string columnName] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| columnName | Kolumnnamnet. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ICellsDataTablePropertyItemDemo1
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i exempeldata i celler
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(499.99);

            // Exportera dataområde till ICellsDataTable med explicit kast
            ICellsDataTable dataTable = (ICellsDataTable)worksheet.Cells.ExportDataTable(0, 0, 3, 2);

            // Flytta till före den första posten
            dataTable.BeforeFirst();

            Console.WriteLine("Reading data table values:");
            while (dataTable.Next())
            {
                // Åtkomst till Item-egenskapen med kolumnnamn (indexerare)
                string product = dataTable["Product"].ToString();
                double price = Convert.ToDouble(dataTable["Price"]);

                Console.WriteLine($"Item[Product]: {product}, Item[Price]: {price}");
            }

            // Spara arbetsboken
            workbook.Save("ItemPropertyDemo.xlsx");
        }
    }
}
```

### Se även

* interface [ICellsDataTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


