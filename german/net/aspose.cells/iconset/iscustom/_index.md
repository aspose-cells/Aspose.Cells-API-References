---
title: "IconSet.IsCustom"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "IconSet-Eigenschaft. Gibt an, ob der Symbolsatz benutzerdefiniert ist. Standardwert ist false"
type: docs
url: /de/net/aspose.cells/iconset/iscustom/
---
## IconSet.IsCustom property

Gibt an, ob das Symbolset benutzerdefiniert ist. Standardwert ist false.

```csharp
public bool IsCustom { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IconSetPropertyIsCustomDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i * 10);
            }

            // Bedingte Formatierung mit benutzerdefiniertem Symbolsatz hinzufügen
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Bereich für bedingte Formatierung festlegen
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 9;
            area.EndColumn = 0;
            fcs.AddArea(area);

            // Symbolsatz-Bedingung hinzufügen
            int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = fcs[conditionIndex];
            
            // Symbolsatztyp festlegen (unter Verwendung eines gültigen IconSetType)
            condition.IconSet.Type = IconSetType.TrafficLights31;

            // Überprüfen Sie die IsCustom-Eigenschaft (schreibgeschützt)
            Console.WriteLine("Is IconSet custom? " + condition.IconSet.IsCustom);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


