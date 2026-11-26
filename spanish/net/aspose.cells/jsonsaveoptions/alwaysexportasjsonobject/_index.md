---
title: "JsonSaveOptions.AlwaysExportAsJsonObject"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad JsonSaveOptions. Indica si siempre se exporta Excel a JSON como objeto incluso cuando solo hay una hoja de cálculo en el archivo"
type: docs
url: /es/net/aspose.cells/jsonsaveoptions/alwaysexportasjsonobject/
---
## JsonSaveOptions.AlwaysExportAsJsonObject property

Indica si siempre se exporta excel a json como objeto, incluso cuando solo hay una hoja de cálculo en el archivo.

```csharp
public bool AlwaysExportAsJsonObject { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyAlwaysExportAsJsonObjectDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de ejemplo con dos hojas de cálculo
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Establecer algunos datos de ejemplo en la primera hoja de cálculo
            Cells cells = workbook.Worksheets[0].Cells;
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Value");
            cells["A2"].PutValue("Item1");
            cells["B2"].PutValue(100);

            // Configura las opciones de guardado JSON
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.AlwaysExportAsJsonObject = true;
            saveOptions.ExportNestedStructure = true;
            saveOptions.SkipEmptyRows = true;

            // Guardar en un archivo JSON
            string outputPath = "output.json";
            workbook.Save(outputPath, saveOptions);

            // Mostrar el contenido JSON guardado
            string jsonContent = File.ReadAllText(outputPath);
            Console.WriteLine(jsonContent);
        }
    }
}
```

### Ver también

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


