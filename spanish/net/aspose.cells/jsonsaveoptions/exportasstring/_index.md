---
title: "JsonSaveOptions.ExportAsString"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad JsonSaveOptions. Exporta el valor de cadena de las celdas a json"
type: docs
url: /es/net/aspose.cells/jsonsaveoptions/exportasstring/
---
## JsonSaveOptions.ExportAsString property

Exporta el valor de cadena de las celdas a json.

```csharp
public bool ExportAsString { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyExportAsStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Crear datos de ejemplo con valores numéricos
            cells["A1"].PutValue("Age");
            cells["B1"].PutValue("Score");
            cells["A2"].PutValue(30);
            cells["B2"].PutValue(95.5);

            JsonSaveOptions exportOptions = new JsonSaveOptions();
            exportOptions.ExportAsString = true;

            string jsonOutput = JsonUtility.ExportRangeToJson(cells.CreateRange("A1:B2"), exportOptions);
            Console.WriteLine("Exported JSON with ExportAsString=true:\n" + jsonOutput);
        }
    }
}
```

### Ver también

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


