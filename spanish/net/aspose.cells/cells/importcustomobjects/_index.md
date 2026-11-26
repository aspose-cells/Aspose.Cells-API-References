---
title: "Cells.ImportCustomObjects"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Importa objetos personalizados"
type: docs
url: /es/net/aspose.cells/cells/importcustomobjects/
---
## ImportCustomObjects(ICollection, string[], bool, int, int, int, bool, string, bool) {#importcustomobjects_1}

Importa objetos personalizados.

```csharp
public int ImportCustomObjects(ICollection list, string[] propertyNames, bool isPropertyNameShown, 
    int firstRow, int firstColumn, int rowNumber, bool insertRows, string dateFormatString, 
    bool convertStringToNumber)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| lista | ICollection | El objeto personalizado |
| propertyNames | String[] | Los nombres de propiedad. Si es nulo, importaremos todas las propiedades del objeto. |
| isPropertyNameShown | Booleano | Indica si el nombre de la propiedad se importará a la primera fila. |
| firstRow | Int32 | El número de fila de la primera celda en la que importar. |
| firstColumn | Int32 | El número de columna de la primera celda en la que importar. |
| rowNumber | Int32 | Número de filas a importar. |
| insertRows | Booleano | Indica si se añaden filas extra para ajustar los datos. |
| dateFormatString | String | Cadena de formato de fecha para celdas. |
| convertStringToNumber | Booleano | Indica si este método intentará convertir la cadena a número. |

### Valor de retorno

Número total de filas importadas.

### Observaciones

Los objetos personalizados deben ser del mismo tipo.

### Ejemplos

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

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportCustomObjects(ICollection, int, int, ImportTableOptions) {#importcustomobjects}

Importa objetos personalizados.

```csharp
public int ImportCustomObjects(ICollection list, int firstRow, int firstColumn, 
    ImportTableOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| lista | ICollection | El objeto personalizado |
| firstRow | Int32 | El número de fila de la primera celda en la que importar. |
| firstColumn | Int32 | El número de columna de la primera celda en la que importar. |
| opciones | ImportTableOptions | Las opciones de importación. |

### Valor de retorno

Número total de filas importadas.

### Observaciones

Los objetos personalizados deben ser del mismo tipo.

### Ejemplos

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

### Ver también

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


