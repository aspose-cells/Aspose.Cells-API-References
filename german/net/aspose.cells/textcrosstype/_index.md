---
title: "Enum TextCrossType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.TextCrossType enum. Enumeriert den Anzeigetyp für Text, wenn die Textbreite größer als die Zellbreite ist."
type: docs
url: /de/net/aspose.cells/textcrosstype/
---
## TextCrossType enumeration

Enumeriert die Anzeigetextart, wenn die Textbreite größer als die Zellenbreite ist.

```csharp
public enum TextCrossType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Default | `1` | Text wie in Microsoft Excel anzeigen. |
| CrossKeep | `2` | Den gesamten Text anzeigen, indem andere Zellen überkreuzt werden, und den Text der überkreuzten Zellen beibehalten. |
| CrossOverride | `3` | Den gesamten Text anzeigen, indem andere Zellen überkreuzt werden, und den Text der überkreuzten Zellen überschreiben. |
| StrictInCell | `4` | Nur den Text innerhalb der Zellbreite anzeigen. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class CellsClassTextCrossTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieltext in einer Zelle festlegen, die überlaufen könnte
            worksheet.Cells["A1"].PutValue("This is a long text that might overflow the cell");
            
            // Bild- oder Druckoptionen erstellen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // Verschiedene TextCrossType-Einstellungen demonstrieren
            options.TextCrossType = TextCrossType.Default;
            SaveToImage(workbook, options, "TextCrossType_Default.png");
            
            options.TextCrossType = TextCrossType.CrossKeep;
            SaveToImage(workbook, options, "TextCrossType_CrossKeep.png");
            
            options.TextCrossType = TextCrossType.CrossOverride;
            SaveToImage(workbook, options, "TextCrossType_CrossOverride.png");
            
            options.TextCrossType = TextCrossType.StrictInCell;
            SaveToImage(workbook, options, "TextCrossType_StrictInCell.png");
        }
        
        private static void SaveToImage(Workbook workbook, ImageOrPrintOptions options, string fileName)
        {
            SheetRender sr = new SheetRender(workbook.Worksheets[0], options);
            sr.ToImage(0, fileName);
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


