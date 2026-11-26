---
title: "Enum AdjustFontSizeForRowType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.Slides.AdjustFontSizeForRowType. Representa qué tipo de filas deben ajustarse"
type: docs
url: /es/net/aspose.cells.slides/adjustfontsizeforrowtype/
---
## AdjustFontSizeForRowType enumeration

Representa qué tipo de filas deben ajustarse.

```csharp
public enum AdjustFontSizeForRowType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | Sin ajuste. |
| EmptyRows | `1` | Si la fila está vacía, cambie el tamaño de fuente para que se ajuste a la altura de la fila. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slides;

namespace AsposeCellsExamples
{
    public class SlidesClassAdjustFontSizeForRowTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rellenar algunos datos en la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // Crear una instancia de PptxSaveOptions con la configuración AdjustFontSizeForRowType
            PptxSaveOptions saveOptions = new PptxSaveOptions
            {
                AdjustFontSizeForRowType = AdjustFontSizeForRowType.EmptyRows
            };

            // Guardar el libro de trabajo como un archivo PPTX
            workbook.Save("AdjustFontSizeForRowTypeDemo.pptx", saveOptions);
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Slides](../../aspose.cells.slides/)
* assembly [Aspose.Cells](../../)


