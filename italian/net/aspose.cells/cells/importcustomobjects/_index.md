---
title: "Cells.ImportCustomObjects"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Importa oggetti personalizzati"
type: docs
url: /it/net/aspose.cells/cells/importcustomobjects/
---
## ImportCustomObjects(ICollection, string[], bool, int, int, int, bool, string, bool) {#importcustomobjects_1}

Importa oggetti personalizzati.

```csharp
public int ImportCustomObjects(ICollection list, string[] propertyNames, bool isPropertyNameShown, 
    int firstRow, int firstColumn, int rowNumber, bool insertRows, string dateFormatString, 
    bool convertStringToNumber)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| elenco | ICollection | L'oggetto personalizzato |
| propertyNames | String[] | I nomi delle proprietà. Se è null, importeremo tutte le proprietà dell'oggetto. |
| isPropertyNameShown | Booleano | Indica se il nome della proprietà verrà importato nella prima riga. |
| firstRow | Int32 | Il numero di riga della prima cella in cui importare. |
| firstColumn | Int32 | Il numero di colonna della prima cella in cui importare. |
| rowNumber | Int32 | Numero di righe da importare. |
| insertRows | Booleano | Indica se vengono aggiunte righe extra per adattare i dati. |
| dateFormatString | String | Stringa di formato data per le celle. |
| convertStringToNumber | Booleano | Indica se questo metodo proverà a convertire la stringa in numero. |

### Valore di ritorno

Numero totale di righe importate.

### Osservazioni

Gli oggetti personalizzati devono essere dello stesso tipo.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections.Generic;

    public class CellsMethodImportCustomObjectsWithICollectionStringBooleanInt3Demo
    {
        public class Product
        {
            public string Name { get; set; }
            public decimal Price { get; set; }
            public int Stock { get; set; }
            public DateTime Date { get; set; }
        }

        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            List<Product> products = new List<Product>
            {
                new Product { Name = "Apple", Price = 2.99m, Stock = 150, Date = new DateTime(2023, 12, 31) },
                new Product { Name = "Orange", Price = 1.99m, Stock = 200, Date = new DateTime(2024, 1, 15) }
            };

            string[] propertyNames = { "Name", "Price", "Stock", "Date" };

            try
            {
                int importedRows = worksheet.Cells.ImportCustomObjects(
                    products,
                    propertyNames,
                    true,
                    0,
                    0,
                    products.Count,
                    true,
                    "yyyy-MM-dd",
                    true
                );

                Console.WriteLine($"Successfully imported {importedRows} rows");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportCustomObjects: {ex.Message}");
            }

            workbook.Save("ImportCustomObjectsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportCustomObjects(ICollection, int, int, ImportTableOptions) {#importcustomobjects}

Importa oggetti personalizzati.

```csharp
public int ImportCustomObjects(ICollection list, int firstRow, int firstColumn, 
    ImportTableOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| elenco | ICollection | L'oggetto personalizzato |
| firstRow | Int32 | Il numero di riga della prima cella in cui importare. |
| firstColumn | Int32 | Il numero di colonna della prima cella in cui importare. |
| opzioni | ImportTableOptions | Le opzioni di importazione. |

### Valore di ritorno

Numero totale di righe importate.

### Osservazioni

Gli oggetti personalizzati devono essere dello stesso tipo.

### Esempi

```csharp
using System;
using System.Collections;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class Customer
    {
        public int CustomerId { get; set; }
        public string Name { get; set; }
    }

    public class CellsMethodImportCustomObjectsWithICollectionInt32Int32ImportTabDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            List<Customer> customerList = new List<Customer>();

            for (int i = 0; i < 5; i++)
            {
                customerList.Add(new Customer
                {
                    CustomerId = i,
                    Name = "Customer" + i
                });
            }

            ImportTableOptions options = new ImportTableOptions
            {
                IsFieldNameShown = false,
                TotalRows = customerList.Count,
                InsertRows = true,
                DateFormat = "dd/mm/yyyy",
                ConvertNumericData = true,
                CheckMergedCells = true
            };

            wb.Worksheets[0].Cells.ImportCustomObjects((ICollection)customerList, 1, 0, options);
            wb.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


