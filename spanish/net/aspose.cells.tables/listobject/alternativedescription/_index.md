---
title: "ListObject.AlternativeDescription"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListObject. Obtiene y establece la descripción alternativa"
type: docs
url: /es/net/aspose.cells.tables/listobject/alternativedescription/
---
## ListObject.AlternativeDescription property

Obtiene y establece la descripción alternativa.

```csharp
public string AlternativeDescription { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyAlternativeDescriptionDemo
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
            
            // Establecer texto alternativo y descripción
            listObject.AlternativeText = "Test";
            listObject.AlternativeDescription = "aSXADCS";

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");

            // Recargar y verificar las propiedades
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            ListObject loadedListObject = loadedWorkbook.Worksheets[0].ListObjects[0];
            
            Console.WriteLine("AlternativeText: " + loadedListObject.AlternativeText);
            Console.WriteLine("AlternativeDescription: " + loadedListObject.AlternativeDescription);
        }
    }
}
```

### Ver también

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


