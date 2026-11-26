---
title: "DocxSaveOptions.AsNormalView"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DocxSaveOptions. Exportar el archivo Excel a docx como vista normal. Si esta propiedad es true, se generará un Área y no se aplicará escala. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/docxsaveoptions/asnormalview/
---
## DocxSaveOptions.AsNormalView property

Exportando archivo de Excel a docx como vista normal. Si esta propiedad es verdadera, se generará una Área y no se aplicará escala. El valor predeterminado es falso.

```csharp
public bool AsNormalView { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DocxSaveOptionsPropertyAsNormalViewDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceda a la primera hoja de cálculo y agregue datos de ejemplo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Normal View Demo";

            try
            {
                // Inicialice DocxSaveOptions
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // Mostrar el valor predeterminado de la propiedad AsNormalView
                Console.WriteLine("Default AsNormalView value: " + saveOptions.AsNormalView);

                // Establecer AsNormalView a true para demostrar su uso
                saveOptions.AsNormalView = true;
                Console.WriteLine("AsNormalView set to: " + saveOptions.AsNormalView);

                // Guarde el libro de trabajo como DOCX con las opciones configuradas
                workbook.Save("AsNormalViewDemo.docx", saveOptions);
                Console.WriteLine("Document saved successfully with AsNormalView option.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


