---
title: "PptxSaveOptions.PptxSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor de PptxSaveOptions. Representa las opciones de guardado pptx"
type: docs
url: /es/net/aspose.cells/pptxsaveoptions/pptxsaveoptions/
---
## PptxSaveOptions() {#constructor}

Representa las opciones de guardado pptx.

```csharp
public PptxSaveOptions()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PptxSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Visible Data");
            worksheet.Cells["A2"].PutValue("Hidden Data");
            worksheet.Cells["B1"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            
            // Ocultar la segunda fila
            worksheet.Cells.Rows[1].IsHidden = true;

            // Crear PptxSaveOptions usando el constructor
            PptxSaveOptions saveOptions = new PptxSaveOptions();
            saveOptions.IgnoreHiddenRows = true;

            // Guardar el libro de trabajo a PPTX con opciones
            workbook.Save("output.pptx", saveOptions);
            
            Console.WriteLine("Workbook saved to PPTX with hidden rows ignored.");
        }
    }
}
```

### Ver también

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PptxSaveOptions(bool) {#constructor_1}

Representa las opciones de guardado de un archivo .pptx.

```csharp
public PptxSaveOptions(bool saveAsImage)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| saveAsImage | Booleano | Si es True, el libro de trabajo se convertirá en algunas imágenes del archivo .pptx. Si es False, el libro de trabajo se convertirá en algunas tablas del archivo .pptx. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Slides;
    using System;

    public class PptxSaveOptionsMethodCtorWithBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(DateTime.Now);

            try
            {
                // Llamar al método #ctor con un parámetro booleano
                bool saveAsImage = true;
                PptxSaveOptions options = new PptxSaveOptions(saveAsImage);

                // Establecer propiedades adicionales
                options.IgnoreHiddenRows = true;
                options.ExportViewType = SlideViewType.View;

                // Guardar el libro de trabajo con opciones PPTX
                workbook.Save("PptxSaveOptionsCtorDemo.pptx", options);

                Console.WriteLine("PptxSaveOptions constructor executed successfully with parameter: " + saveAsImage);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing PptxSaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


