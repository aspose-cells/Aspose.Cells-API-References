---
title: "ImageOrPrintOptions.DefaultEditLanguage"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageOrPrintOptions-Eigenschaft. Gibt die Standardsprache für die Bearbeitung zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells.rendering/imageorprintoptions/defaulteditlanguage/
---
## ImageOrPrintOptions.DefaultEditLanguage property

Liest oder setzt die Standardsprache für die Bearbeitung.

```csharp
public DefaultEditLanguage DefaultEditLanguage { get; set; }
```

### Hinweise

Es kann unterschiedliche Layouts für Textabsätze anzeigen/rendern, wenn verschiedene Bearbeitungssprachen festgelegt sind. Standard ist Auto.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Setze die Standardschriftart der Arbeitsmappe auf eine, die CJK‑Zeichen unterstützt
            workbook.DefaultStyle.Font.Name = "MS Gothic";
            
            // Setze japanischen Text, der ein korrektes Umbrechen erfordert
            string japaneseText = "日本語のテキストサンプル：これは折り返し表示のテストです。長いテキストをセル内で適切に表示するか確認します。";
            sheet.Cells["A1"].Value = japaneseText;
            
            // Konfiguriere die Zellenformatierung – korrigiert mit dem richtigen Eigenschaftsnamen
            Cell cell = sheet.Cells["A1"];
            Style style = cell.GetStyle();
            style.IsTextWrapped = true;  // Correct property name for text wrapping
            cell.SetStyle(style);
            
            sheet.Cells.SetColumnWidth(0, 15);
            sheet.Cells.SetRowHeight(0, 60);

            // Bildrenderoptionen erstellen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.DefaultEditLanguage = DefaultEditLanguage.CJK;
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.CheckWorkbookDefaultFont = true;

            // Render das Arbeitsblatt zu einem Bild
            SheetRender renderer = new SheetRender(sheet, options);
            renderer.ToImage(0, "CJK_Text_Rendering.png");
            
            Console.WriteLine("Generated image with CJK text rendering.");
        }
    }
}
```

### Siehe auch

* enum [DefaultEditLanguage](../../../aspose.cells/defaulteditlanguage/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


