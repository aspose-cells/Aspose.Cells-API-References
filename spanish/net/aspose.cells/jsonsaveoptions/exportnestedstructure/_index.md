---
title: "JsonSaveOptions.ExportNestedStructure"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad JsonSaveOptions. Exportado como estructura Json de jerarquía padre-hijo"
type: docs
url: /es/net/aspose.cells/jsonsaveoptions/exportnestedstructure/
---
## JsonSaveOptions.ExportNestedStructure property

Exportado como estructura Json jerárquica padre-hijo.

```csharp
public bool ExportNestedStructure { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyExportNestedStructureDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de ejemplo con datos anidados
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear estructura de datos anidada
            worksheet.Cells["A1"].PutValue("Parent");
            worksheet.Cells["B1"].PutValue("Child");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["B2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Fruits");
            worksheet.Cells["B3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Vegetables");
            worksheet.Cells["B4"].PutValue("Carrot");

            // Configura las opciones de guardado JSON con ExportNestedStructure
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.ExportNestedStructure = true;
            saveOptions.AlwaysExportAsJsonObject = true;

            // Guardar con estructura anidada
            string outputPath = "output_nested.json";
            workbook.Save(outputPath, saveOptions);

            Console.WriteLine("Workbook exported to JSON with nested structure. Output: " + outputPath);
        }
    }
}
```

### Ver también

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


