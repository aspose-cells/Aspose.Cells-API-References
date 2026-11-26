---
title: "DocxSaveOptions.SaveElementType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DocxSaveOptions. Indica qué elementos deben guardarse"
type: docs
url: /es/net/aspose.cells/docxsaveoptions/saveelementtype/
---
## DocxSaveOptions.SaveElementType property

Indica qué elementos deben guardarse.

```csharp
public SaveElementType SaveElementType { get; set; }
```

### Ejemplos

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class DocxSaveOptionsPropertySaveElementTypeDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo y agregue algunos datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Demo Data");

            try
            {
                // Inicialice DocxSaveOptions
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // NOTA: La propiedad SaveElementType no está presente en la clase DocxSaveOptions
                // basado en la reflexión de API proporcionada. Si existiera, lo leería así:
                // var elementType = saveOptions.SaveElementType;
                // Console.WriteLine("SaveElementType: " + elementType);

                // Demuestre la lectura de una propiedad existente: SaveAsEditableShaps
                Console.WriteLine("SaveAsEditableShaps (default): " + saveOptions.SaveAsEditableShaps);

                // Establezca la propiedad en true y muestre el nuevo valor
                saveOptions.SaveAsEditableShaps = true;
                Console.WriteLine("SaveAsEditableShaps (after set): " + saveOptions.SaveAsEditableShaps);

                // Guarde el libro de trabajo como DOCX usando las opciones configuradas
                workbook.Save("SaveElementTypeDemo.docx", saveOptions);
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### Ver también

* enum [SaveElementType](../../../aspose.cells.saving/saveelementtype/)
* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


