---
title: "IconSet.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà IconSet. Ottieni o imposta il tipo di set di icone da visualizzare. Impostare il tipo verificherà automaticamente se il conteggio corrente di Cfvoss è conforme al nuovo tipo. Se non è conforme, le vecchie Cfvos verranno rimosse e verranno aggiunte le Cfvos predefinite."
type: docs
url: /it/net/aspose.cells/iconset/type/
---
## IconSet.Type property

Ottieni o imposta il tipo di set di icone da visualizzare. Impostare il tipo verificherà automaticamente se il conteggio corrente di Cfods è coerente con il nuovo tipo. Se non è coerente, i Cfods vecchi saranno rimossi e verranno aggiunti i Cfods predefiniti.

```csharp
public IconSetType Type { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IconSetPropertyTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            int idx = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition cond = fcs[idx];
            IconSet iconSet = cond.IconSet;

            // Dimostra l'uso della proprietà Type
            iconSet.Type = IconSetType.Arrows3;

            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(120);
            sheet.Cells["A3"].PutValue(260);

            workbook.Save("IconSetExample.xlsx");
        }
    }
}
```

### Vedi anche

* enum [IconSetType](../../iconsettype/)
* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


