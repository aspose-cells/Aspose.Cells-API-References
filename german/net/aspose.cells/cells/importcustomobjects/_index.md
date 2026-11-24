---
title: "Cells.ImportCustomObjects"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Importiert benutzerdefinierte Objekte"
type: docs
url: /de/net/aspose.cells/cells/importcustomobjects/
---
## ImportCustomObjects(ICollection, string[], bool, int, int, int, bool, string, bool) {#importcustomobjects_1}

Importiert benutzerdefinierte Objekte.

```csharp
public int ImportCustomObjects(ICollection list, string[] propertyNames, bool isPropertyNameShown, 
    int firstRow, int firstColumn, int rowNumber, bool insertRows, string dateFormatString, 
    bool convertStringToNumber)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Liste | ICollection | Das benutzerdefinierte Objekt |
| propertyNames | String[] | Die Eigenschaftsnamen. Wenn es null ist, importieren wir alle Eigenschaften des Objekts. |
| isPropertyNameShown | Boolean | Gibt an, ob der Property-Name in die erste Zeile importiert wird. |
| firstRow | Int32 | Die Zeilennummer der ersten Zelle, in die importiert werden soll. |
| firstColumn | Int32 | Die Spaltennummer der ersten Zelle, in die importiert werden soll. |
| rowNumber | Int32 | Anzahl der zu importierenden Zeilen. |
| insertRows | Boolean | Gibt an, ob zusätzliche Zeilen hinzugefügt werden, um die Daten anzupassen. |
| dateFormatString | String | Datumsformatzeichenfolge für Zellen. |
| convertStringToNumber | Boolean | Gibt an, ob diese Methode versucht, einen String in eine Zahl zu konvertieren. |

### Rückgabewert

Gesamtzahl der importierten Zeilen.

### Hinweise

Die benutzerdefinierten Objekte sollten vom gleichen Typ sein.

### Beispiele

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

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportCustomObjects(ICollection, int, int, ImportTableOptions) {#importcustomobjects}

Importiert benutzerdefinierte Objekte.

```csharp
public int ImportCustomObjects(ICollection list, int firstRow, int firstColumn, 
    ImportTableOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Liste | ICollection | Das benutzerdefinierte Objekt |
| firstRow | Int32 | Die Zeilennummer der ersten Zelle, in die importiert werden soll. |
| firstColumn | Int32 | Die Spaltennummer der ersten Zelle, in die importiert werden soll. |
| Optionen | ImportTableOptions | Die Importoptionen. |

### Rückgabewert

Gesamtzahl der importierten Zeilen.

### Hinweise

Die benutzerdefinierten Objekte sollten vom gleichen Typ sein.

### Beispiele

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

### Siehe auch

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


