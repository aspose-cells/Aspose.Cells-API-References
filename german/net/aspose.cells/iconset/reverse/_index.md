---
title: "IconSet.Reverse"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "IconSet-Eigenschaft. Gibt das Flag zurück oder setzt es, das angibt, ob die Standardreihenfolge der Symbole in diesem Symbolsatz umgekehrt wird. Standardwert ist false"
type: docs
url: /de/net/aspose.cells/iconset/reverse/
---
## IconSet.Reverse property

Abrufen oder Festlegen des Flags, das angibt, ob die Standardreihenfolge der Symbole in diesem Symbolset umgekehrt wird. Standardwert ist false.

```csharp
public bool Reverse { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IconSetPropertyReverseDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Bedingte Formatierung hinzufügen
            ConditionalFormattingCollection cfs = worksheet.ConditionalFormattings;
            int index = cfs.Add();
            FormatConditionCollection cf = cfs[index];
            
            // Bereich festlegen
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 4;
            area.StartColumn = 0;
            area.EndColumn = 0;
            cf.AddArea(area);

            // Bedingte Formatierung für Symbolsatz erstellen
            cf.AddCondition(FormatConditionType.IconSet);
            IconSet iconSet = cf[0].IconSet;
            
            // Symbolsatz konfigurieren
            iconSet.Type = IconSetType.Arrows3;
            iconSet.ShowValue = true;
            
            // Reverse-Eigenschaft demonstrieren
            Console.WriteLine("Original IconSet Reverse value: " + iconSet.Reverse);
            iconSet.Reverse = true;
            Console.WriteLine("Modified IconSet Reverse value: " + iconSet.Reverse);

            // Speichere die Arbeitsmappe
            workbook.Save("IconSetPropertyReverseDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


