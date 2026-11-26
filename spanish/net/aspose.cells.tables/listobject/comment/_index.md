---
title: "ListObject.Comment"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de ListObject. Obtiene y establece el comentario de la tabla"
type: docs
url: /es/net/aspose.cells.tables/listobject/comment/
---
## ListObject.Comment property

Obtiene y establece el comentario de la tabla.

```csharp
public string Comment { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyCommentDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear datos de ejemplo para el objeto de lista
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(100);

            // Crear un objeto de lista
            int index = worksheet.ListObjects.Add(0, 0, 1, 1, true);
            ListObject listObj = worksheet.ListObjects[index];

            // Establecer y demostrar la propiedad Comment
            listObj.Comment = "This is a sample comment for the list object";
            Console.WriteLine("List Object Comment: " + listObj.Comment);

            // Redimensionar el objeto de lista para incluir más datos
            listObj.Resize(0, 0, 2, 1, true);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue(200);

            // Guarda el libro de trabajo
            workbook.Save("ListObjectCommentDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


