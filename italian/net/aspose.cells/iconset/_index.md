---
title: "Classe IconSet"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.IconSet. Descrivi la regola di formattazione condizionale IconSet. Questa regola di formattazione condizionale applica icone alle celle in base ai loro valori"
type: docs
url: /it/net/aspose.cells/iconset/
---
## IconSet class

Descrive la regola di formattazione condizionale IconSet. Questa regola di formattazione condizionale applica icone alle celle in base ai loro valori.

```csharp
public class IconSet
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CfIcons](../../aspose.cells/iconset/cficons/) { get; } | Ottieni il [`ConditionalFormattingIcon`](../conditionalformattingicon/) dalla collezione |
| [Cfvos](../../aspose.cells/iconset/cfvos/) { get; } | Ottieni l'istanza CFValueObjects. |
| [IsCustom](../../aspose.cells/iconset/iscustom/) { get; } | Indica se il set di icone è personalizzato. Il valore predefinito è false. |
| [Reverse](../../aspose.cells/iconset/reverse/) { get; set; } | Ottieni o imposta il flag che indica se invertire l'ordine predefinito delle icone in questo set di icone. Il valore predefinito è false. |
| [ShowValue](../../aspose.cells/iconset/showvalue/) { get; set; } | Ottieni o imposta il flag che indica se mostrare i valori delle celle a cui è applicato questo set di icone. Il valore predefinito è true. |
| [Type](../../aspose.cells/iconset/type/) { get; set; } | Ottieni o imposta il tipo di set di icone da visualizzare. Impostare il tipo verificherà automaticamente se il conteggio corrente di Cfods è coerente con il nuovo tipo. Se non è coerente, i Cfods vecchi saranno rimossi e verranno aggiunti i Cfods predefiniti. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IconSetDemo
    {
        public static void IconSetExample()
        {
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiunge una formattazione condizionale vuota
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Imposta l'intervallo di formattazione condizionale
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            // Aggiunge condizione
            int idx = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition cond = fcs[idx];

            // Ottieni Icon Set
            IconSet iconSet = cond.IconSet;

            // Imposta tipo di icona
            iconSet.Type = IconSetType.Arrows3;

            // Imposta proprietà aggiuntive
            iconSet.ShowValue = true;
            iconSet.Reverse = false;

            // Inserisci valori delle celle
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(120);
            sheet.Cells["A3"].PutValue(260);

            // Salvataggio del file Excel
            workbook.Save("IconSetExample.xlsx");
            workbook.Save("IconSetExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


