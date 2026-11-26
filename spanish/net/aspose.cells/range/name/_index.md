---
title: "Range.Name"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Range. Obtiene o establece el nombre del rango"
type: docs
url: /es/net/aspose.cells/range/name/
---
## Range.Name property

Obtiene o establece el nombre del rango.

```csharp
public string Name { get; set; }
```

### Observaciones

Los rangos con nombre son compatibles. Por ejemplo,

range.Name = "Sheet1!MyRange";

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear un rango (columnas A a B)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 2, true);
            
            // Establecer la propiedad de nombre para el rango
            range.Name = "testRange";
            
            // Verificar que el nombre se haya establecido
            Console.WriteLine("Range name: " + range.Name);
            
            // Guarda el libro de trabajo
            workbook.Save("RangeWithName.xlsx");
            
            // Abrir el archivo guardado para demostrar que el nombre persiste
            Workbook loadedWorkbook = new Workbook("RangeWithName.xlsx");
            Aspose.Cells.Range loadedRange = loadedWorkbook.Worksheets[0].Cells.CreateRange(0, 2, true);
            Console.WriteLine("Loaded range name: " + loadedRange.Name);
        }
    }
}
```

### Ver también

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


