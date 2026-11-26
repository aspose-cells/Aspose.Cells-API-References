---
title: "CellWatch.CellName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CellWatch. Obtiene y establece el nombre de la celda"
type: docs
url: /es/net/aspose.cells/cellwatch/cellname/
---
## CellWatch.CellName property

Obtiene y establece el nombre de la celda.

```csharp
public string CellName { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellWatchPropertyCellNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunas observaciones de celda
            worksheet.CellWatches.Add("B5");
            worksheet.CellWatches.Add("C10");
            
            // Mostrar los nombres de celda de todas las observaciones
            Console.WriteLine("Cell Watches:");
            foreach (CellWatch watch in worksheet.CellWatches)
            {
                Console.WriteLine(watch.CellName);
            }
            
            // Agregar una nueva observación y mostrar su nombre
            worksheet.CellWatches.Add("A1");
            Console.WriteLine("Added new watch: " + 
                worksheet.CellWatches[worksheet.CellWatches.Count - 1].CellName);
            
            // Guarda el libro de trabajo
            workbook.Save("CellWatchDemo.xlsx");
        }
    }
}
```

### Ver también

* class [CellWatch](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


