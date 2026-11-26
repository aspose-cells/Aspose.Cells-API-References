---
title: "Range.Worksheet"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Range. Obtiene el Worksheetobject que contiene este rango"
type: docs
url: /es/net/aspose.cells/range/worksheet/
---
## Range.Worksheet property

Obtiene el objeto `Worksheet` que contiene este rango.

```csharp
public Worksheet Worksheet { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyWorksheetDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear un rango con nombre
            worksheet.Cells["A1"].PutValue("Test");
            worksheet.Cells["B1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            
            // Define un rango con nombre
            int index = workbook.Worksheets.Names.Add("MyRange");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet1!$A$1:$B$2";
            
            // Obtén el rango por nombre (califica completamente Range para evitar ambigüedad)
            Aspose.Cells.Range range = workbook.Worksheets.GetRangeByName("MyRange");
            
            // Demostrar el uso de la propiedad Worksheet
            Console.WriteLine("Range belongs to worksheet: " + range.Worksheet.Name);
            
            // Usar la propiedad Worksheet para modificar celdas
            range.Worksheet.Cells["A1"].PutValue("Updated");
            
            // Guarda el libro de trabajo
            workbook.Save("RangePropertyWorksheetDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Worksheet](../../worksheet/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


