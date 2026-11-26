---
title: "ListObject.ShowTableStyleRowStripes"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de ListObject. Indica si se aplica el formato de franjas de fila a"
type: docs
url: /es/net/aspose.cells.tables/listobject/showtablestylerowstripes/
---
## ListObject.ShowTableStyleRowStripes property

Indica si se aplica formato de franjas de fila.

```csharp
public bool ShowTableStyleRowStripes { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyShowTableStyleRowStripesDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("Item3");
            worksheet.Cells["B4"].PutValue(300);

            // Crear un objeto de lista
            ListObjectCollection listObjects = worksheet.ListObjects;
            int index = listObjects.Add("A1", "B4", true);
            ListObject listObject = listObjects[index];

            // Demostrar la propiedad ShowTableStyleRowStripes
            Console.WriteLine("Before: ShowTableStyleRowStripes = " + listObject.ShowTableStyleRowStripes);
            listObject.ShowTableStyleRowStripes = false;
            Console.WriteLine("After: ShowTableStyleRowStripes = " + listObject.ShowTableStyleRowStripes);

            // Guarda el libro de trabajo
            workbook.Save("ListObjectShowTableStyleRowStripesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


