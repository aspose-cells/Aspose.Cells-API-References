---
title: "WorksheetCollection.ActiveSheetIndex"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorksheetCollection. Representa el índice de la hoja activa cuando se abre la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/worksheetcollection/activesheetindex/
---
## WorksheetCollection.ActiveSheetIndex property

Representa el índice de la hoja de cálculo activa cuando se abre la hoja de cálculo.

```csharp
public int ActiveSheetIndex { get; set; }
```

### Observaciones

El índice de la hoja se basa en cero.

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyActiveSheetIndexDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con 3 hojas de cálculo
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Establecer el índice de la hoja activa a 1 (segunda hoja)
            workbook.Worksheets.ActiveSheetIndex = 1;

            // Verificar la hoja activa
            Console.WriteLine("Active Sheet: " + workbook.Worksheets[workbook.Worksheets.ActiveSheetIndex].Name);

            // Guarda el libro de trabajo
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "ActiveSheetDemo.xlsx");
            workbook.Save(outputPath);

            Console.WriteLine("File saved to: " + outputPath);
        }
    }
}
```

### Ver también

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


