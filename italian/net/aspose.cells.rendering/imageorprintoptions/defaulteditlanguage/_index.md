---
title: "ImageOrPrintOptions.DefaultEditLanguage"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageOrPrintOptions. Ottiene o imposta la lingua di modifica predefinita"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/defaulteditlanguage/
---
## ImageOrPrintOptions.DefaultEditLanguage property

Ottiene o imposta la lingua di modifica predefinita.

```csharp
public DefaultEditLanguage DefaultEditLanguage { get; set; }
```

### Osservazioni

Può visualizzare/renderizzare layout diversi per il paragrafo di testo quando è impostata una lingua di modifica diversa. Il valore predefinito è Auto.

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Imposta il font predefinito della cartella di lavoro su uno che supporta i caratteri CJK
            workbook.DefaultStyle.Font.Name = "MS Gothic";
            
            // Imposta il testo giapponese che richiederà un corretto a capo
            string japaneseText = "日本語のテキストサンプル：これは折り返し表示のテストです。長いテキストをセル内で適切に表示するか確認します。";
            sheet.Cells["A1"].Value = japaneseText;
            
            // Configura la formattazione delle celle - corretto usando il nome della proprietà corretto
            Cell cell = sheet.Cells["A1"];
            Style style = cell.GetStyle();
            style.IsTextWrapped = true;  // Correct property name for text wrapping
            cell.SetStyle(style);
            
            sheet.Cells.SetColumnWidth(0, 15);
            sheet.Cells.SetRowHeight(0, 60);

            // Creare le opzioni di rendering dell'immagine
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.DefaultEditLanguage = DefaultEditLanguage.CJK;
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.CheckWorkbookDefaultFont = true;

            // Renderizza il foglio di lavoro in immagine
            SheetRender renderer = new SheetRender(sheet, options);
            renderer.ToImage(0, "CJK_Text_Rendering.png");
            
            Console.WriteLine("Generated image with CJK text rendering.");
        }
    }
}
```

### Vedi anche

* enum [DefaultEditLanguage](../../../aspose.cells/defaulteditlanguage/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


