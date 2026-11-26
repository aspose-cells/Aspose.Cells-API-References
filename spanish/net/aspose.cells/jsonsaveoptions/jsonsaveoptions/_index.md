---
title: "JsonSaveOptions.JsonSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor JsonSaveOptions. Crea opciones para guardar un archivo json"
type: docs
url: /es/net/aspose.cells/jsonsaveoptions/jsonsaveoptions/
---
## JsonSaveOptions constructor

Crea opciones para guardar el archivo json.

```csharp
public JsonSaveOptions()
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Datos de ejemplo para exportar como JSON
            workbook.Worksheets[0].Cells["A1"].PutValue("Name");
            workbook.Worksheets[0].Cells["B1"].PutValue("Age");
            workbook.Worksheets[0].Cells["A2"].PutValue("John");
            workbook.Worksheets[0].Cells["B2"].PutValue(30);
            
            // Inicializa JsonSaveOptions usando el constructor
            JsonSaveOptions options = new JsonSaveOptions();
            
            // Establece las opciones de exportación JSON
            options.ExportNestedStructure = true;
            options.SkipEmptyRows = true;
            options.ValidateMergedAreas = true;
            
            // Guarda el libro de trabajo con opciones JSON
            string outputPath = "output.json";
            workbook.Save(outputPath, options);
            
            Console.WriteLine("JSON file saved successfully with options.");
        }
    }
}
```

### Ver también

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


