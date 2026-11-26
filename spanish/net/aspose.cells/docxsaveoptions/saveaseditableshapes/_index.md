---
title: "DocxSaveOptions.SaveAsEditableShapes"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DocxSaveOptions. Guardar todos los objetos de dibujo como formas editables en el archivo Word para que pueda editarlos en Word"
type: docs
url: /es/net/aspose.cells/docxsaveoptions/saveaseditableshapes/
---
## DocxSaveOptions.SaveAsEditableShapes property

Guarda todos los objetos de dibujo como formas editables en el archivo de Word, para que puedas editarlos en Word.

```csharp
public bool SaveAsEditableShapes { get; set; }
```

### Observaciones

Solo para gráficos.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DocxSaveOptionsPropertySaveAsEditableShapesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceda a la primera hoja de cálculo y agregue datos de ejemplo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Editable Shapes Demo";

            try
            {
                // Inicialice DocxSaveOptions
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // Mostrar el valor predeterminado de la propiedad SaveAsEditableShapes
                Console.WriteLine("Default SaveAsEditableShapes value: " + saveOptions.SaveAsEditableShapes);

                // Establecer SaveAsEditableShapes a true para demostrar su uso
                saveOptions.SaveAsEditableShapes = true;
                Console.WriteLine("SaveAsEditableShapes set to: " + saveOptions.SaveAsEditableShapes);

                // Guarde el libro de trabajo como DOCX con las opciones configuradas
                workbook.Save("SaveAsEditableShapesDemo.docx", saveOptions);
                Console.WriteLine("Document saved successfully with SaveAsEditableShapes option.");
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


