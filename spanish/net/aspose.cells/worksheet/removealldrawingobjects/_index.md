---
title: "Worksheet.RemoveAllDrawingObjects"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de Worksheet. Elimina todos los objetos de dibujo en esta hoja de cálculo"
type: docs
url: /es/net/aspose.cells/worksheet/removealldrawingobjects/
---
## Worksheet.RemoveAllDrawingObjects method

Elimina todos los objetos de dibujo en esta hoja de cálculo.

```csharp
public void RemoveAllDrawingObjects()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodRemoveAllDrawingObjectsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos objetos de dibujo a la hoja de cálculo
            worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 50);
            worksheet.Shapes.AddLine(1, 0, 5, 100, 5, 150);
            
            // Guardar antes de eliminar los objetos
            workbook.Save("BeforeRemove.xlsx", SaveFormat.Xlsx);
            
            // Eliminar todos los objetos de dibujo
            worksheet.RemoveAllDrawingObjects();
            
            // Guardar después de eliminar los objetos
            workbook.Save("AfterRemove.xlsx", SaveFormat.Xlsx);
            
            // Liberar el libro de trabajo
            workbook.Dispose();
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


