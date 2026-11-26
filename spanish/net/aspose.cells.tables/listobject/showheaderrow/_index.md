---
title: "ListObject.ShowHeaderRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListObject. Obtiene y establece si esta Tabla muestra la fila de encabezado"
type: docs
url: /es/net/aspose.cells.tables/listobject/showheaderrow/
---
## ListObject.ShowHeaderRow property

Obtiene y establece si esta Tabla muestra la fila de encabezado.

```csharp
public bool ShowHeaderRow { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyShowHeaderRowDemo
    {
        public static void Run()
        {
            // Crea un libro de trabajo y una hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");

            // Crear un objeto de lista o tabla
            int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 0, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.TableStyleType = TableStyleType.TableStyleMedium2;
            table.ShowHeaderRow = true; // Header row is visible by default

            Console.WriteLine("Header row is visible: " + table.ShowHeaderRow);
            Console.WriteLine("Header cell value: " + worksheet.Cells["A1"].StringValue);

            // Ocultar la fila de encabezado
            table.ShowHeaderRow = false;
            Console.WriteLine("\nAfter setting ShowHeaderRow to false:");
            Console.WriteLine("Header row is visible: " + table.ShowHeaderRow);
            Console.WriteLine("Header cell value: " + worksheet.Cells["A1"].StringValue);

            // Guarda el libro de trabajo
            workbook.Save("ListObjectShowHeaderRowDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


