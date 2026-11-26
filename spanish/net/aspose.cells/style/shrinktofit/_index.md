---
title: "Style.ShrinkToFit"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Style. Representa si el texto se reduce automáticamente para ajustarse al ancho de columna disponible"
type: docs
url: /es/net/aspose.cells/style/shrinktofit/
---
## Style.ShrinkToFit property

Representa si el texto se reduce automáticamente para ajustarse al ancho de columna disponible.

```csharp
public bool ShrinkToFit { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyShrinkToFitDemo
    {
        public static void Run()
        {
            // Crear un objeto libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Acceder a la colección de celdas
            Cells cells = worksheet.Cells;
            
            // Establecer texto en la celda A1 que sea más largo que el ancho de la columna
            cells["A1"].PutValue("This is a long text that needs shrinking to fit");
            
            // Establecer el ancho de columna para que sea menor que la longitud del texto
            cells.SetColumnWidth(0, 10);
            
            // Obtener el estilo de la celda A1
            Style style = cells["A1"].GetStyle();
            
            // Establecer ShrinkToFit a true
            style.ShrinkToFit = true;
            
            // Aplicar el estilo a la celda A1
            cells["A1"].SetStyle(style);
            
            // Guarda el libro de trabajo
            workbook.Save("ShrinkToFitDemo.xlsx");
            
            Console.WriteLine("ShrinkToFit demo completed successfully.");
        }
    }
}
```

### Ver también

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


