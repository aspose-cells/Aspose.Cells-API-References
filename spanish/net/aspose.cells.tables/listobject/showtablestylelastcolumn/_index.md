---
title: "ListObject.ShowTableStyleLastColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListObject. Indica si la última columna de la tabla es a la que se aplica el estilo"
type: docs
url: /es/net/aspose.cells.tables/listobject/showtablestylelastcolumn/
---
## ListObject.ShowTableStyleLastColumn property

Indica si la última columna de la tabla tiene el estilo aplicado.

```csharp
public bool ShowTableStyleLastColumn { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyShowTableStyleLastColumnDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B4"].PutValue(1.2);

            // Crear un objeto de lista
            ListObjectCollection listObjects = worksheet.ListObjects;
            int index = listObjects.Add("A1", "B4", true);
            ListObject listObject = listObjects[index];

            // Establecer la propiedad ShowTableStyleLastColumn
            listObject.ShowTableStyleLastColumn = true;

            // Guarda el libro de trabajo
            workbook.Save("ListObjectShowLastColumnStyle.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("File saved with ShowTableStyleLastColumn enabled.");
        }
    }
}
```

### Ver también

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


