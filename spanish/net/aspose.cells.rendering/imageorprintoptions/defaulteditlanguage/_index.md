---
title: "ImageOrPrintOptions.DefaultEditLanguage"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. Obtiene o establece el idioma de edición predeterminado"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/defaulteditlanguage/
---
## ImageOrPrintOptions.DefaultEditLanguage property

Obtiene o establece el idioma de edición predeterminado.

```csharp
public DefaultEditLanguage DefaultEditLanguage { get; set; }
```

### Observaciones

Puede mostrar/renderizar diferentes diseños para párrafos de texto cuando se establece un idioma de edición diferente. El predeterminado es Auto.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyDefaultEditLanguageDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Establezca la fuente predeterminada del libro de trabajo a una que admita caracteres CJK
            workbook.DefaultStyle.Font.Name = "MS Gothic";
            
            // Establezca texto japonés que requiera un ajuste adecuado
            string japaneseText = "日本語のテキストサンプル：これは折り返し表示のテストです。長いテキストをセル内で適切に表示するか確認します。";
            sheet.Cells["A1"].Value = japaneseText;
            
            // Configure el formato de celda - corregido usando el nombre de propiedad correcto
            Cell cell = sheet.Cells["A1"];
            Style style = cell.GetStyle();
            style.IsTextWrapped = true;  // Correct property name for text wrapping
            cell.SetStyle(style);
            
            sheet.Cells.SetColumnWidth(0, 15);
            sheet.Cells.SetRowHeight(0, 60);

            // Crear opciones de renderizado de imagen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.DefaultEditLanguage = DefaultEditLanguage.CJK;
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.CheckWorkbookDefaultFont = true;

            // Renderiza la hoja de cálculo a una imagen
            SheetRender renderer = new SheetRender(sheet, options);
            renderer.ToImage(0, "CJK_Text_Rendering.png");
            
            Console.WriteLine("Generated image with CJK text rendering.");
        }
    }
}
```

### Ver también

* enum [DefaultEditLanguage](../../../aspose.cells/defaulteditlanguage/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


