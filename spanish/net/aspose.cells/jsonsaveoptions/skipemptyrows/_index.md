---
title: "JsonSaveOptions.SkipEmptyRows"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad JsonSaveOptions. Indica si se omiten filas vacías"
type: docs
url: /es/net/aspose.cells/jsonsaveoptions/skipemptyrows/
---
## JsonSaveOptions.SkipEmptyRows property

Indica si se omiten filas vacías.

```csharp
public bool SkipEmptyRows { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertySkipEmptyRowsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Datos de ejemplo - agrega algunas celdas con valores y deja algunas filas vacías
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            // Deja la fila 3 vacía
            worksheet.Cells["A4"].PutValue("Data3");
            worksheet.Cells["B4"].PutValue("Data4");

            // Configura las opciones de guardado JSON con SkipEmptyRows
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.SkipEmptyRows = true; // This will skip the empty row 3
            
            // Guardar en JSON
            string outputPath = "output.json";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("JSON saved with SkipEmptyRows=true. Empty rows were skipped.");
        }
    }
}
```

### Ver también

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


