---
title: "FormatCondition.IconSet"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FormatCondition. Ottieni l'istanza IconSet della formattazione condizionale. L'istanza predefinita IconSetType è TrafficLights31. Valido solo per il tipo IconSet"
type: docs
url: /it/net/aspose.cells/formatcondition/iconset/
---
## FormatCondition.IconSet property

Ottieni l'istanza "IconSet" della formattazione condizionale. Il tipo IconSetType dell'istanza predefinita è TrafficLights31. Valida solo per type = IconSet.

```csharp
public IconSet IconSet { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyIconSetDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            for (int i = 0; i < 10; i++)
            {
                sheet.Cells[i, 0].PutValue(i * 10);
            }

            // Aggiungi formattazione condizionale
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
            
            // Imposta l'intervallo di celle
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcs.AddArea(area);

            // Aggiungi condizione e imposta il tipo su IconSet
            int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = fcs[conditionIndex];
            
            // Ottieni l'IconSet e configurarlo
            IconSet iconSet = condition.IconSet;
            iconSet.Type = IconSetType.TrafficLights31;
            iconSet.ShowValue = true;
            iconSet.Reverse = false;

            // Salva la cartella di lavoro
            workbook.Save("IconSetDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [IconSet](../../iconset/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


