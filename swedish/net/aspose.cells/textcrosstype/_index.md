---
title: "Enum TextCrossType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.TextCrossType enum. Enumererar visningstyp för text när textens bredd är större än cellens bredd"
type: docs
url: /sv/net/aspose.cells/textcrosstype/
---
## TextCrossType enumeration

Enumererar visningstyp för text när textbredden är större än cellbredden.

```csharp
public enum TextCrossType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Default | `1` | Visa text som i Microsoft Excel. |
| CrossKeep | `2` | Visa all text genom att korsa andra celler och behålla texten i de korsade cellerna. |
| CrossOverride | `3` | Visa all text genom att korsa andra celler och skriva över texten i de korsade cellerna. |
| StrictInCell | `4` | Visa endast texten inom cellens bredd. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ange exempeltext i en cell som kan flöda över
            worksheet.Cells["A1"].PutValue("This is a long text that might overflow the cell");
            
            // Skapa bild- eller utskriftsalternativ
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // Demonstrera olika TextCrossType-inställningar
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

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


