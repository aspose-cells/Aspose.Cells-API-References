---
title: "ListObject.QueryTable"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListObject. Obtiene la QueryTable vinculada"
type: docs
url: /es/net/aspose.cells.tables/listobject/querytable/
---
## ListObject.QueryTable property

Obtiene la QueryTable vinculada.

```csharp
public QueryTable QueryTable { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListObjectPropertyQueryTableDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Crear un objeto de lista
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = worksheet.ListObjects[index];

            try
            {
                // Acceder a la propiedad QueryTable (solo lectura)
                QueryTable queryTable = listObject.QueryTable;

                if (queryTable != null)
                {
                    // Mostrar propiedades de QueryTable
                    Console.WriteLine("QueryTable Name: " + queryTable.Name);
                    Console.WriteLine("Connection ID: " + queryTable.ConnectionId);
                    Console.WriteLine("Preserve Formatting: " + queryTable.PreserveFormatting);
                    Console.WriteLine("Adjust Column Width: " + queryTable.AdjustColumnWidth);

                    // Acceder al rango de resultados si está disponible
                    if (queryTable.ResultRange != null)
                    {
                        Console.WriteLine("Result Range Address: " + queryTable.ResultRange.Name);
                    }
                }
                else
                {
                    Console.WriteLine("No QueryTable associated with this ListObject");
                }

                // Guarda el libro de trabajo
                workbook.Save("QueryTableDemo.xlsx");
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

* class [QueryTable](../../../aspose.cells/querytable/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


