---
title: "IconFilter.IconSetType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "IconFilter-Eigenschaft. Liest und setzt, welches Symbolset für dieses Filterkriterium verwendet wird."
type: docs
url: /de/net/aspose.cells/iconfilter/iconsettype/
---
## IconFilter.IconSetType property

Liest und setzt, welches Symbolset für dieses Filterkriterium verwendet wird.

```csharp
public IconSetType IconSetType { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IconFilterPropertyIconSetTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten befüllen
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i * 10);
            }

            // Automatischen Filter erstellen
            worksheet.AutoFilter.Range = "A1:A10";
            FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
            filterColumn.FilterType = FilterType.IconFilter;

            // Liest den Symbolfilter
            IconFilter iconFilter = (IconFilter)filterColumn.Filter;

            // Aktuellen IconSetType anzeigen (Standard ist None)
            Console.WriteLine("Current IconSetType: " + iconFilter.IconSetType);

            // Auf das 3-Pfeile-Symbolset setzen
            iconFilter.IconSetType = IconSetType.Arrows3;
            iconFilter.IconId = 1; // Show only middle arrow

            // Bedingte Formatierung anwenden, um die Symbole darzustellen
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection formatConditionCollection = conditionalFormattings[index];
            int conditionIndex = formatConditionCollection.AddCondition(FormatConditionType.IconSet);
            FormatCondition formatCondition = formatConditionCollection[conditionIndex];
            formatCondition.IconSet.Type = IconSetType.Arrows3;
            
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            formatConditionCollection.AddArea(area);

            // Auf das Ampel-Symbolset ändern
            iconFilter.IconSetType = IconSetType.TrafficLights31;
            iconFilter.IconId = 2; // Show only green light

            // Ergebnis speichern
            workbook.Save("PropertyIconSetTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [IconSetType](../../iconsettype/)
* class [IconFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


