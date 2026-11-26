---
title: "XlsSaveOptions.IsTemplate"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad XlsSaveOptions. Indica si se está guardando un archivo de plantilla"
type: docs
url: /es/net/aspose.cells/xlssaveoptions/istemplate/
---
## XlsSaveOptions.IsTemplate property

Indica si se está guardando un archivo de plantilla.

```csharp
[Obsolete("Use XlsSaveOptions(SaveFormat.Xlt) when it is template, otherwise use XlsSaveOptions().")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsTemplate { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, cree XlsSaveOptions con el formato de guardado correspondiente (xlt para true y xls para false). Este método será eliminado 12 meses después, desde agosto de 2020. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsSaveOptionsPropertyIsTemplateDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar datos de muestra a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Template");
            
            // Guardar como archivo de plantilla
            string outputPath = "output_template.xlt";
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            saveOptions.IsTemplate = true;
            
            using (FileStream fs = File.Create(outputPath))
            {
                workbook.Save(fs, saveOptions);
            }
            
            // Verificar el formato del archivo guardado
            Workbook loadedWorkbook = new Workbook(outputPath);
            Console.WriteLine("File format: " + loadedWorkbook.FileFormat);
        }
    }
}
```

### Ver también

* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


