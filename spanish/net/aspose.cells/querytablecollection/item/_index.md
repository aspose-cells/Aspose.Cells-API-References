---
title: "QueryTableCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad QueryTableCollection. Obtiene la tabla de consulta por el índice específico"
type: docs
url: /es/net/aspose.cells/querytablecollection/item/
---
## QueryTableCollection indexer

Obtiene la querytable por el índice específico.

```csharp
public QueryTable this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice. |

### Valor de retorno

La tabla de consulta

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTableCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder a QueryTableCollection
            QueryTableCollection queryTables = worksheet.QueryTables;

            try
            {
                // Comprobar si hay alguna QueryTable
                if (queryTables.Count > 0)
                {
                    // Acceder a la primera QueryTable usando la propiedad Item
                    QueryTable firstQueryTable = queryTables[0];
                    Console.WriteLine("First QueryTable accessed successfully.");

                    // Mostrar algunas propiedades de la QueryTable
                    Console.WriteLine("QueryTable Name: " + firstQueryTable.Name);
                }
                else
                {
                    Console.WriteLine("No QueryTables found in the worksheet.");
                }

                // Guarda el libro de trabajo
                workbook.Save("QueryTableItemDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [QueryTable](../../querytable/)
* class [QueryTableCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


