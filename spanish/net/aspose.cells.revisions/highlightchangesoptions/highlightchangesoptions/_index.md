---
title: "HighlightChangesOptions.HighlightChangesOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor HighlightChangesOptions. Representa opciones para resaltar revisiones o cambios de archivos Excel compartidos"
type: docs
url: /es/net/aspose.cells.revisions/highlightchangesoptions/highlightchangesoptions/
---
## HighlightChangesOptions constructor

Representa opciones de resaltado de revisiones o cambios de archivos de Excel compartidos.

```csharp
public HighlightChangesOptions(bool highlightOnScreen, bool listOnNewSheet)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| highlightOnScreen | Booleano | Indica si se resaltan los cambios en pantalla. |
| listOnNewSheet | Booleano | Indica si se listan los cambios en una nueva hoja de cálculo. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class HighlightChangesOptionsMethodCtorWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar algunos datos de ejemplo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Original Value");
            worksheet.Cells["A2"].PutValue(100);
            
            // Crear HighlightChangesOptions con parámetros booleanos
            HighlightChangesOptions options = new HighlightChangesOptions(true, true);
            
            // Simular el seguimiento de cambios (normalmente tendrías revisiones reales)
            Console.WriteLine("HighlightChangesOptions created with:");
            Console.WriteLine($"First parameter (show changes): {true}");
            Console.WriteLine($"Second parameter (changes on new sheet): {true}");
            
            // Guarda el libro de trabajo
            workbook.Save("HighlightChangesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [HighlightChangesOptions](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


