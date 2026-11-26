---
title: "PptxSaveOptions.AdjustFontSizeForRowType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de PptxSaveOptions. Representa qué tipo de línea necesita ajustar el tamaño de fuente si la altura de la fila es pequeña"
type: docs
url: /es/net/aspose.cells/pptxsaveoptions/adjustfontsizeforrowtype/
---
## PptxSaveOptions.AdjustFontSizeForRowType property

Representa qué tipo de línea necesita ajustar el tamaño de fuente si la altura de la fila es pequeña.

```csharp
public AdjustFontSizeForRowType AdjustFontSizeForRowType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slides;

namespace AsposeCellsExamples
{
    public class PptxSaveOptionsPropertyAdjustFontSizeForRowTypeDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos datos y filas vacías
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data 1");
            worksheet.Cells["A3"].PutValue(""); // Empty row
            worksheet.Cells["A4"].PutValue("Data 2");
            
            // Crear opciones de guardado PPTX
            PptxSaveOptions saveOptions = new PptxSaveOptions();
            saveOptions.AdjustFontSizeForRowType = AdjustFontSizeForRowType.EmptyRows;
            
            // Guardar a PPTX
            workbook.Save("output.pptx", saveOptions);
            
            Console.WriteLine("File saved with AdjustFontSizeForRowType setting");
        }
    }
}
```

### Ver también

* enum [AdjustFontSizeForRowType](../../../aspose.cells.slides/adjustfontsizeforrowtype/)
* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


