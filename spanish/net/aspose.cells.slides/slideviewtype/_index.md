---
title: "Enum SlideViewType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.Slides.SlideViewType. Representa el tipo al exportar a diapositivas"
type: docs
url: /es/net/aspose.cells.slides/slideviewtype/
---
## SlideViewType enumeration

Representa el tipo al exportar a diapositivas.

```csharp
public enum SlideViewType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| View | `0` | Exportando como vista en MS Excel. |
| Print | `1` | Exportando como impresión. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slides;

namespace AsposeCellsExamples
{
    public class SlidesClassSlideViewTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Slide 1 Content");
            worksheet.Cells["A2"].PutValue("This will appear in the exported slides");

            // Configurar opciones de guardado PPTX con SlideViewType
            PptxSaveOptions saveOptions = new PptxSaveOptions
            {
                ExportViewType = SlideViewType.Print,
                OnePagePerSheet = true
            };

            // Guardar como PPTX
            workbook.Save("SlidesViewTypeDemo.pptx", saveOptions);
            
            Console.WriteLine("PPTX file created with SlideViewType.Print");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Slides](../../aspose.cells.slides/)
* assembly [Aspose.Cells](../../)


