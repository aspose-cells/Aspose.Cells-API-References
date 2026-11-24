---
title: "FormatCondition.IconSet"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormatCondition-Eigenschaft. Holen Sie die IconSet-Instanz der bedingten Formatierung. Der Standard-IconSetType ist TrafficLights31. Gültig nur für den Typ IconSet"
type: docs
url: /de/net/aspose.cells/formatcondition/iconset/
---
## FormatCondition.IconSet property

Rufen Sie die "IconSet"-Instanz der bedingten Formatierung ab. Der IconSetType der Standardinstanz ist TrafficLights31. Gültig nur für Typ = IconSet.

```csharp
public IconSet IconSet { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyIconSetDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            for (int i = 0; i < 10; i++)
            {
                sheet.Cells[i, 0].PutValue(i * 10);
            }

            // Bedingte Formatierung hinzufügen
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
            
            // Legen Sie den Zellenbereich fest
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcs.AddArea(area);

            // Fügen Sie eine Bedingung hinzu und setzen Sie den Typ auf IconSet
            int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = fcs[conditionIndex];
            
            // Holen Sie das IconSet und konfigurieren Sie es
            IconSet iconSet = condition.IconSet;
            iconSet.Type = IconSetType.TrafficLights31;
            iconSet.ShowValue = true;
            iconSet.Reverse = false;

            // Speichere die Arbeitsmappe
            workbook.Save("IconSetDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [IconSet](../../iconset/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


