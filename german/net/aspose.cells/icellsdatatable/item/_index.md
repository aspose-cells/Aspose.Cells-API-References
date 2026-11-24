---
title: "ICellsDataTable.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ICellsDataTable-Eigenschaft. Gibt die in der durch den Index angegebenen Spalte gespeicherten Daten zurück"
type: docs
url: /de/net/aspose.cells/icellsdatatable/item/
---
## ICellsDataTable indexer (1 of 2)

Gibt die in der durch den Index angegebenen Spalte gespeicherten Daten zurück.

```csharp
public object this[int columnIndex] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| columnIndex | Der nullbasierte Index der Spalte. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ICellsDataTablePropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle ein benutzerdefiniertes ICellsDataTable mit Beispieldaten
            ICellsDataTable dataTable = new SampleDataTable();

            // Cursor-Position zurücksetzen
            dataTable.BeforeFirst();

            Console.WriteLine("Reading data using Item property:");
            while (dataTable.Next())
            {
                // Werte über Spaltenindex zugreifen
                Console.WriteLine($"Product: {dataTable[0]}, Price: {dataTable[1]}, Stock: {dataTable[2]}");

                // Werte über Spaltennamen zugreifen
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

### Siehe auch

* interface [ICellsDataTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ICellsDataTable indexer (2 of 2)

Ruft die in der durch den Spaltennamen angegebenen Spalte gespeicherten Daten ab.

```csharp
public object this[string columnName] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| columnName | Der Spaltenname. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ICellsDataTablePropertyItemDemo1
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten in Zellen einfügen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(499.99);

            // Exportiere den Datenbereich zu ICellsDataTable mit explizitem Cast
            ICellsDataTable dataTable = (ICellsDataTable)worksheet.Cells.ExportDataTable(0, 0, 3, 2);

            // Zur Position vor dem ersten Datensatz bewegen
            dataTable.BeforeFirst();

            Console.WriteLine("Reading data table values:");
            while (dataTable.Next())
            {
                // Greife auf die Item-Eigenschaft über Spaltennamen (Indexer) zu
                string product = dataTable["Product"].ToString();
                double price = Convert.ToDouble(dataTable["Price"]);

                Console.WriteLine($"Item[Product]: {product}, Item[Price]: {price}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("ItemPropertyDemo.xlsx");
        }
    }
}
```

### Siehe auch

* interface [ICellsDataTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


