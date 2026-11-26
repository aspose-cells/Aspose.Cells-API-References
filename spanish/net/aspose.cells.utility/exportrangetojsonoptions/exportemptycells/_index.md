---
title: "ExportRangeToJsonOptions.ExportEmptyCells"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExportRangeToJsonOptions. Indica si se exportan celdas vacías como null"
type: docs
url: /es/net/aspose.cells.utility/exportrangetojsonoptions/exportemptycells/
---
## ExportRangeToJsonOptions.ExportEmptyCells property

Indica si se exportan celdas vacías como null.

```csharp
public bool ExportEmptyCells { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class ExportRangeToJsonOptionsPropertyExportEmptyCellsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos datos a las celdas
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            // Dejar B2 vacío intencionalmente
            
            // Crear opciones de exportación y habilitar la exportación de celdas vacías
            ExportRangeToJsonOptions exportOptions = new ExportRangeToJsonOptions();
            exportOptions.ExportEmptyCells = true;
            
            // Exportar el rango a JSON
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 2, 2);
            string jsonData = JsonUtility.ExportRangeToJson(range, exportOptions);
            
            Console.WriteLine(jsonData);
        }
    }
}
```

### Ver también

* class [ExportRangeToJsonOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


