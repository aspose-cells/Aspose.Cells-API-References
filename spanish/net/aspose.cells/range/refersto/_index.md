---
title: "Range.RefersTo"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Range. Obtiene los rangos a los que se refiere"
type: docs
url: /es/net/aspose.cells/range/refersto/
---
## Range.RefersTo property

Obtiene a qué se refiere el rango.

```csharp
public string RefersTo { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyRefersToDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos datos a las celdas
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            
            // Crear un rango con nombre
            int index = workbook.Worksheets.Names.Add("MyRange");
            Name name = workbook.Worksheets.Names[index];
            
            // Establece la propiedad RefersTo para el rango con nombre
            name.RefersTo = "=Sheet1!$A$1:$A$3";
            
            // Obtén los rangos referidos por el nombre
            Aspose.Cells.Range[] ranges = name.GetRanges();
            
            // Muestra la propiedad RefersTo del primer rango
            Console.WriteLine("Named range refers to: " + ranges[0].RefersTo);
            
            // Crea una fórmula que use el rango con nombre
            worksheet.Cells["B1"].Formula = "=SUM(MyRange)";
            
            // Calcular la fórmula
            Console.WriteLine("Sum of named range: " + worksheet.Cells["B1"].Value);
        }
    }
}
```

### Ver también

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


