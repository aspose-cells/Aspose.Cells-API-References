---
title: "ListObject.AlternativeText"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de ListObject. Obtiene y establece el texto alternativo"
type: docs
url: /es/net/aspose.cells.tables/listobject/alternativetext/
---
## ListObject.AlternativeText property

Obtiene y establece el texto alternativo.

```csharp
public string AlternativeText { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyAlternativeTextDemo
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

            // Crear un objeto de lista o tabla
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];
            
            // Establecer texto alternativo y descripción
            table.AlternativeText = "Test";
            table.AlternativeDescription = "aSXADCS";
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
            
            // Recargar y verificar
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            ListObject loadedTable = loadedWorkbook.Worksheets[0].ListObjects[0];
            
            Console.WriteLine("AlternativeText: " + loadedTable.AlternativeText);
            Console.WriteLine("AlternativeDescription: " + loadedTable.AlternativeDescription);
        }
    }
}
```

### Ver también

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


