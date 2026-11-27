---
title: "Cells.ImportCustomObjects"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Importerar anpassade objekt"
type: docs
url: /sv/net/aspose.cells/cells/importcustomobjects/
---
## ImportCustomObjects(ICollection, string[], bool, int, int, int, bool, string, bool) {#importcustomobjects_1}

Importerar anpassade objekt.

```csharp
public int ImportCustomObjects(ICollection list, string[] propertyNames, bool isPropertyNameShown, 
    int firstRow, int firstColumn, int rowNumber, bool insertRows, string dateFormatString, 
    bool convertStringToNumber)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| lista | ICollection | Det anpassade objektet |
| propertyNames | String[] | Egenskapsnamnen. Om den är null, importerar vi alla egenskaper för objektet. |
| isPropertyNameShown | Boolean | Indikerar om egenskapsnamnet kommer att importeras till den första raden. |
| firstRow | Int32 | Radnumret för den första cellen att importera i. |
| firstColumn | Int32 | Kolumnnumret för den första cellen att importera i. |
| rowNumber | Int32 | Antal rader att importera. |
| insertRows | Boolean | Indikerar om extra rader läggs till för att passa data. |
| dateFormatString | String | Datumformatsträng för celler. |
| convertStringToNumber | Boolean | Indikerar om denna metod kommer att försöka konvertera sträng till tal. |

### Returvärde

Totalt antal importerade rader.

### Anmärkningar

De anpassade objekten bör vara av samma typ.

### Exempel

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

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportCustomObjects(ICollection, int, int, ImportTableOptions) {#importcustomobjects}

Importerar anpassade objekt.

```csharp
public int ImportCustomObjects(ICollection list, int firstRow, int firstColumn, 
    ImportTableOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| lista | ICollection | Det anpassade objektet |
| firstRow | Int32 | Radnumret för den första cellen att importera i. |
| firstColumn | Int32 | Kolumnnumret för den första cellen att importera i. |
| alternativ | ImportTableOptions | Importalternativen. |

### Returvärde

Totalt antal importerade rader.

### Anmärkningar

De anpassade objekten bör vara av samma typ.

### Exempel

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

### Se även

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


