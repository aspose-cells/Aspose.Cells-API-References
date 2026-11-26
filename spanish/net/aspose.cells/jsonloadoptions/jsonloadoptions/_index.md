---
title: "JsonLoadOptions.JsonLoadOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor de JsonLoadOptions. Crea una opción para cargar el archivo"
type: docs
url: /es/net/aspose.cells/jsonloadoptions/jsonloadoptions/
---
## JsonLoadOptions constructor

Crea una opción de carga del archivo.

```csharp
public JsonLoadOptions()
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Directorios de origen y salida
            string sourceDir = "SourceDir/";
            string outputDir = "OutputDir/";
            
            // Crear JsonLoadOptions usando el constructor
            JsonLoadOptions loadOptions = new JsonLoadOptions();
            loadOptions.KeptSchema = true;

            // Cargar archivo JSON con opciones
            Workbook workbook = new Workbook(sourceDir + "example.json", loadOptions);
            
            // Guardar como archivo Excel
            workbook.Save(outputDir + "example.xlsx");

            // Guardar de nuevo en JSON con JsonSaveOptions
            workbook.Save(outputDir + "example_output.json", new JsonSaveOptions()
            {
                ExportNestedStructure = true,
                SkipEmptyRows = true
            });

            Console.WriteLine("JSON to Excel conversion completed successfully.");
        }
    }
}
```

### Ver también

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


