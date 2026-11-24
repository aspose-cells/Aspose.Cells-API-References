---
title: "DataSorterKey.IconId"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataSorterKey-Eigenschaft. Stellt die ID des Symbolsatztyps dar"
type: docs
url: /de/net/aspose.cells/datasorterkey/iconid/
---
## DataSorterKey.IconId property

Stellt die ID des Symbolsatztyps dar.

```csharp
public int IconId { get; }
```

### Hinweise

Wirkt nur, wenn [`Type`](../type/) Icon ist.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataSorterKeyPropertyIconIdDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten mit Werten hinzufügen, die Symbolsätze nutzen könnten
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Fügen Sie eine bedingte Formatierung für das Symbolset hinzu
            ConditionalFormattingCollection cfc = worksheet.ConditionalFormattings;
            int index = cfc.Add();
            FormatConditionCollection fcc = cfc[index];
            CellArea area = CellArea.CreateCellArea("A1", "A5");
            fcc.AddArea(area);
            fcc.AddCondition(FormatConditionType.IconSet);
            fcc[0].IconSet.Type = IconSetType.Arrows3;

            // Erstellen Sie einen DataSorter und fügen Sie einen Schlüssel hinzu
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);

            // Daten sortieren
            sorter.Sort(worksheet.Cells, area);

            try
            {
                // Die IconId-Eigenschaft der Sortierschlüssel anzeigen
                foreach (DataSorterKey key in sorter.Keys)
                {
                    Console.WriteLine($"IconId: {key.IconId}");
                    Console.WriteLine($"IconSetType: {key.IconSetType}");
                }

                // Speichere die Arbeitsmappe
                workbook.Save("IconIdDemo.xlsx");
                Console.WriteLine("IconId demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


