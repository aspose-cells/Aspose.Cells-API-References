---
title: "ConditionalFormattingIcon.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ConditionalFormattingIcon-Eigenschaft. Liest und schreibt den Symbolset-Typ"
type: docs
url: /de/net/aspose.cells/conditionalformattingicon/type/
---
## ConditionalFormattingIcon.Type property

Liefert und setzt den Symbolsettyp.

```csharp
public IconSetType Type { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingIconPropertyTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Bedingte Formatierung mit Symbolsatz hinzufügen
            ConditionalFormattingCollection cfs = worksheet.ConditionalFormattings;
            int index = cfs.Add();
            FormatConditionCollection fc = cfs[index];
            fc.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 2, EndColumn = 0 });
            
            int conditionIndex = fc.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = fc[conditionIndex];
            condition.IconSet.Type = IconSetType.Symbols3;
            
            // Formatierung anwenden und berechnen
            workbook.CalculateFormula();

            // Formatierungsergebnis abrufen und Type-Eigenschaft demonstrieren
            Cell cell = worksheet.Cells["A2"];
            ConditionalFormattingResult formattingResult = cell.GetConditionalFormattingResult();
            
            Console.WriteLine("Icon Set Type: " + formattingResult.ConditionalFormattingIcon.Type);
            Console.WriteLine("Icon Index: " + formattingResult.ConditionalFormattingIcon.Index);
        }
    }
}
```

### Siehe auch

* enum [IconSetType](../../iconsettype/)
* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


