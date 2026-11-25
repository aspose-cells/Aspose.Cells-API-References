---
title: "IconSet.IsCustom"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà IconSet. Indica se il set di icone è personalizzato. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/iconset/iscustom/
---
## IconSet.IsCustom property

Indica se il set di icone è personalizzato. Il valore predefinito è false.

```csharp
public bool IsCustom { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IconSetPropertyIsCustomDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i * 10);
            }

            // Aggiungi formattazione condizionale con set di icone personalizzato
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Imposta l'intervallo per la formattazione condizionale
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 9;
            area.EndColumn = 0;
            fcs.AddArea(area);

            // Aggiungi condizione al set di icone
            int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = fcs[conditionIndex];
            
            // Imposta il tipo di set di icone (usando un IconSetType valido)
            condition.IconSet.Type = IconSetType.TrafficLights31;

            // Verifica la proprietà IsCustom (sola lettura)
            Console.WriteLine("Is IconSet custom? " + condition.IconSet.IsCustom);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


