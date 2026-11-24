---
title: "Klasse ConditionalFormattingIcon"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ConditionalFormattingIcon Klasse. Stellt das benutzerdefinierte Symbol einer bedingten Formatierungsregel dar"
type: docs
url: /de/net/aspose.cells/conditionalformattingicon/
---
## ConditionalFormattingIcon class

Stellt das benutzerdefinierte Symbol einer bedingten Formatierungsregel dar.

```csharp
public class ConditionalFormattingIcon
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ImageData](../../aspose.cells/conditionalformattingicon/imagedata/) { get; } | Liefert die Symbolset-Daten. |
| [Index](../../aspose.cells/conditionalformattingicon/index/) { get; set; } | Liefert und setzt den Index des Symbols im Symbolset. |
| [Type](../../aspose.cells/conditionalformattingicon/type/) { get; set; } | Liefert und setzt den Symbolsettyp. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetImageData](../../aspose.cells/conditionalformattingicon/getimagedata/)(Cell) | Liefert die Bilddaten mit den Zelleinstellungen. |
| static [GetIconImageData](../../aspose.cells/conditionalformattingicon/geticonimagedata/)(IconSetType, int) | Rufen Sie die Icon-Set-Daten ab |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingIconDemo
    {
        public static void ConditionalFormattingIconExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greifen Sie auf das erste Arbeitsblatt in der Arbeitsmappe zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Rufen Sie die Sammlung der bedingten Formatierungen ab
            ConditionalFormattingCollection cformattings = worksheet.ConditionalFormattings;
            
            // Fügen Sie der Sammlung eine neue bedingte Formatierung hinzu
            int index = cformattings.Add();
            
            // Greifen Sie auf die Formatbedingungs-Sammlung zu
            FormatConditionCollection fcs = cformattings[index];
            
            // Definieren Sie den Zellbereich, auf den die bedingte Formatierung angewendet werden soll
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 0
            };
            
            // Fügen Sie den Zellbereich zur Formatbedingungs-Sammlung hinzu
            fcs.AddArea(ca);
            
            // Fügen Sie eine Bedingung hinzu, um Icon-Sets zu verwenden
            int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition fc = fcs[conditionIndex];
            
            // Legen Sie den Typ des Icon-Sets fest
            fc.IconSet.Type = IconSetType.Arrows3;

            // Passen Sie die einzelnen Symbole im Icon-Set an
            ConditionalFormattingIcon cfIcon0 = fc.IconSet.CfIcons[0];
            cfIcon0.Type = IconSetType.Arrows3;
            cfIcon0.Index = 0;

            ConditionalFormattingIcon cfIcon1 = fc.IconSet.CfIcons[1];
            cfIcon1.Type = IconSetType.ArrowsGray3;
            cfIcon1.Index = 1;

            ConditionalFormattingIcon cfIcon2 = fc.IconSet.CfIcons[2];
            cfIcon2.Type = IconSetType.Boxes5;
            cfIcon2.Index = 2;

            // Speichere die Arbeitsmappe
            workbook.Save("ConditionalFormattingIconExample.xlsx");
            workbook.Save("ConditionalFormattingIconExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


