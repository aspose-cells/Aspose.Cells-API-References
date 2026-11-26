---
title: "ListObject.StartRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListObject. Obtiene la fila inicial del rango"
type: docs
url: /es/net/aspose.cells.tables/listobject/startrow/
---
## ListObject.StartRow property

Obtiene la fila inicial del rango.

```csharp
public int StartRow { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyStartRowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear datos de ejemplo a partir de la fila 2
            worksheet.Cells["A2"].PutValue("ID");
            worksheet.Cells["B2"].PutValue("Name");
            worksheet.Cells["A3"].PutValue(1);
            worksheet.Cells["B3"].PutValue("John");
            worksheet.Cells["A4"].PutValue(2);
            worksheet.Cells["B4"].PutValue("Mary");

            // Crear un objeto de lista a partir de la fila 2
            int listObjectIndex = worksheet.ListObjects.Add(1, 0, 3, 1, true);
            ListObject listObject = worksheet.ListObjects[listObjectIndex];

            // Mostrar la propiedad StartRow
            Console.WriteLine("ListObject StartRow: " + listObject.StartRow);

            // Para "modificar" la fila inicial, necesitamos recrear el ListObject
            worksheet.ListObjects.RemoveAt(listObjectIndex);
            listObjectIndex = worksheet.ListObjects.Add(2, 0, 3, 1, true);
            listObject = worksheet.ListObjects[listObjectIndex];
            
            Console.WriteLine("Modified ListObject StartRow: " + listObject.StartRow);
        }
    }
}
```

### Ver también

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


