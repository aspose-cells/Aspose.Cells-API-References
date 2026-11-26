---
title: "ImageOrPrintOptions.TextCrossType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. Obtiene o establece el tipo de visualización de texto cuando el ancho del texto es mayor que el ancho de la celda"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/textcrosstype/
---
## ImageOrPrintOptions.TextCrossType property

Obtiene o establece el tipo de visualización de texto cuando el ancho del texto es mayor que el ancho de la celda.

```csharp
public TextCrossType TextCrossType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyTextCrossTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer texto largo que excederá el ancho de la celda
            worksheet.Cells["A1"].PutValue("This is a long text that exceeds cell width");
            worksheet.Cells["A1"].GetStyle().ShrinkToFit = false;

            // Crear opciones de imagen o impresión
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // Demostrar diferentes configuraciones de TextCrossType
            options.TextCrossType = TextCrossType.Default;
            SaveAsImage(workbook, options, "TextCrossType_Default.png");

            options.TextCrossType = TextCrossType.CrossKeep;
            SaveAsImage(workbook, options, "TextCrossType_CrossKeep.png");

            options.TextCrossType = TextCrossType.CrossOverride;
            SaveAsImage(workbook, options, "TextCrossType_CrossOverride.png");

            options.TextCrossType = TextCrossType.StrictInCell;
            SaveAsImage(workbook, options, "TextCrossType_StrictInCell.png");
        }

        private static void SaveAsImage(Workbook workbook, ImageOrPrintOptions options, string fileName)
        {
            SheetRender sr = new SheetRender(workbook.Worksheets[0], options);
            sr.ToImage(0, fileName);
        }
    }
}
```

### Ver también

* enum [TextCrossType](../../../aspose.cells/textcrosstype/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


