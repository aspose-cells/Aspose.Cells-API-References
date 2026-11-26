---
title: "Worksheet.ActiveCell"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Worksheet. Obtiene o establece la celda activa en la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/worksheet/activecell/
---
## Worksheet.ActiveCell property

Obtiene o establece la celda activa en la hoja de cálculo.

```csharp
public string ActiveCell { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyActiveCellDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establezca la celda activa a B2
            worksheet.ActiveCell = "B2";
            
            // Imprimir la dirección de la celda activa
            Console.WriteLine("Active Cell: " + worksheet.ActiveCell);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
            
            // Cargar el libro guardado para verificar la celda activa
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("Loaded Active Cell: " + loadedWorkbook.Worksheets[0].ActiveCell);
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


