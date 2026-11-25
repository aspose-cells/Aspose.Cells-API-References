---
title: "ICellsDataTable.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ICellsDataTable. Ottiene i dati memorizzati nella colonna specificata per indice"
type: docs
url: /it/net/aspose.cells/icellsdatatable/item/
---
## ICellsDataTable indexer (1 of 2)

Ottiene i dati memorizzati nella colonna specificata per indice.

```csharp
public object this[int columnIndex] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| columnIndex | L'indice della colonna basato su zero. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ICellsDataTablePropertyItemDemo
    {
        public static void Run()
        {
            // Crea un ICellsDataTable personalizzato con dati di esempio
            ICellsDataTable dataTable = new SampleDataTable();

            // Reimposta la posizione del cursore
            dataTable.BeforeFirst();

            Console.WriteLine("Reading data using Item property:");
            while (dataTable.Next())
            {
                // Accedi ai valori per indice di colonna
                Console.WriteLine($"Product: {dataTable[0]}, Price: {dataTable[1]}, Stock: {dataTable[2]}");

                // Accedi ai valori per nome della colonna
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

### Vedi anche

* interface [ICellsDataTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ICellsDataTable indexer (2 of 2)

Ottiene i dati memorizzati nella colonna specificata per nome della colonna.

```csharp
public object this[string columnName] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| columnName | Il nome della colonna. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ICellsDataTablePropertyItemDemo1
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola dati di esempio nelle celle
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(499.99);

            // Esporta l'intervallo di dati in ICellsDataTable con cast esplicito
            ICellsDataTable dataTable = (ICellsDataTable)worksheet.Cells.ExportDataTable(0, 0, 3, 2);

            // Sposta prima del primo record
            dataTable.BeforeFirst();

            Console.WriteLine("Reading data table values:");
            while (dataTable.Next())
            {
                // Accedi alla proprietà Item usando i nomi delle colonne (indicizzatore)
                string product = dataTable["Product"].ToString();
                double price = Convert.ToDouble(dataTable["Price"]);

                Console.WriteLine($"Item[Product]: {product}, Item[Price]: {price}");
            }

            // Salva la cartella di lavoro
            workbook.Save("ItemPropertyDemo.xlsx");
        }
    }
}
```

### Vedi anche

* interface [ICellsDataTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


