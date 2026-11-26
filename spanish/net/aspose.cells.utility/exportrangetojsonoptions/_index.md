---
title: "Clase ExportRangeToJsonOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Utility.ExportRangeToJsonOptions. Indica las opciones para exportar un rango a json"
type: docs
url: /es/net/aspose.cells.utility/exportrangetojsonoptions/
---
## ExportRangeToJsonOptions class

Indica las opciones para exportar un rango a JSON.

```csharp
public class ExportRangeToJsonOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [ExportRangeToJsonOptions](exportrangetojsonoptions/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ExportAsString](../../aspose.cells.utility/exportrangetojsonoptions/exportasstring/) { get; set; } | Exporta el valor de cadena de las celdas a json. |
| [ExportEmptyCells](../../aspose.cells.utility/exportrangetojsonoptions/exportemptycells/) { get; set; } | Indica si se exportan celdas vacías como null. |
| [HasHeaderRow](../../aspose.cells.utility/exportrangetojsonoptions/hasheaderrow/) { get; set; } | Indica si el rango contiene una fila de encabezado. |
| [Indent](../../aspose.cells.utility/exportrangetojsonoptions/indent/) { get; set; } | Indica la sangría. |

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class UtilityClassExportRangeToJsonOptionsDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Crea opciones de exportación
            var exportOptions = new ExportRangeToJsonOptions();
            
            // Exporta rango a JSON
            var range = worksheet.Cells.CreateRange(0, 0, 3, 2);
            string jsonData = JsonUtility.ExportRangeToJson(range, exportOptions);

            // Genera el JSON
            Console.WriteLine("Exported JSON:");
            Console.WriteLine(jsonData);
            
            // Guardar en archivo (opcional)
            File.WriteAllText("exported_data.json", jsonData);
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


