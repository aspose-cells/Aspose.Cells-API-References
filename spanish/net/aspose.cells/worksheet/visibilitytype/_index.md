---
title: "Worksheet.VisibilityType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Worksheet. Indica el estado visible de esta hoja"
type: docs
url: /es/net/aspose.cells/worksheet/visibilitytype/
---
## Worksheet.VisibilityType property

Indica el estado visible de esta hoja.

```csharp
public VisibilityType VisibilityType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyVisibilityTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar hojas de cálculo
            workbook.Worksheets.Add();
            workbook.Worksheets.Add();

            // Establecer diferentes tipos de visibilidad para cada hoja de cálculo
            workbook.Worksheets[0].VisibilityType = VisibilityType.Hidden;
            workbook.Worksheets[1].VisibilityType = VisibilityType.VeryHidden;
            workbook.Worksheets[2].VisibilityType = VisibilityType.Visible;

            // Guarda el libro de trabajo
            string outputPath = "output_visibility.xlsx";
            workbook.Save(outputPath);

            // Recargar el libro de trabajo para verificar la configuración de visibilidad
            Workbook loadedWorkbook = new Workbook(outputPath);
            
            // Mostrar tipos de visibilidad
            Console.WriteLine("Worksheet 0 Visibility: " + loadedWorkbook.Worksheets[0].VisibilityType);
            Console.WriteLine("Worksheet 1 Visibility: " + loadedWorkbook.Worksheets[1].VisibilityType);
            Console.WriteLine("Worksheet 2 Visibility: " + loadedWorkbook.Worksheets[2].VisibilityType);
        }
    }
}
```

### Ver también

* enum [VisibilityType](../../visibilitytype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


