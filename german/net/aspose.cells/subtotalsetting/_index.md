---
title: "Klasse SubtotalSetting"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.SubtotalSetting‑Klasse. Stellt die Einstellung des Zwischensummens dar."
type: docs
url: /de/net/aspose.cells/subtotalsetting/
---
## SubtotalSetting class

Stellt die Einstellung der Zwischensumme dar.

```csharp
public class SubtotalSetting
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [GroupBy](../../aspose.cells/subtotalsetting/groupby/) { get; } | Das Feld, nach dem gruppiert wird, als nullbasierter ganzzahliger Offset. |
| [SubtotalFunction](../../aspose.cells/subtotalsetting/subtotalfunction/) { get; } | Die Zwischensummen‑Funktion. |
| [SummaryBelowData](../../aspose.cells/subtotalsetting/summarybelowdata/) { get; } | Gibt an, ob eine Zusammenfassung unter den Daten hinzugefügt wird. |
| [TotalList](../../aspose.cells/subtotalsetting/totallist/) { get; } | Ein Array von nullbasierten Feld‑Offsets, das die Felder angibt, zu denen die Zwischensummen hinzugefügt werden. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassSubtotalSettingDemo
    {
        public static void Run()
        {
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Beispieldaten zum Arbeitsblatt hinzufügen
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["B1"].PutValue("Value");
                worksheet.Cells["A2"].PutValue("Group A");
                worksheet.Cells["A3"].PutValue("Group B");
                worksheet.Cells["A4"].PutValue("Group A");
                worksheet.Cells["A5"].PutValue("Group B");
                worksheet.Cells["B2"].PutValue(100);
                worksheet.Cells["B3"].PutValue(200);
                worksheet.Cells["B4"].PutValue(300);
                worksheet.Cells["B5"].PutValue(400);

                // Definieren Sie den Zellbereich für Zwischensummen.
                CellArea area = CellArea.CreateCellArea("A1", "B5");

                // Wenden Sie Zwischensummen auf die Daten an.
                worksheet.Cells.Subtotal(
                    area,
                    0, // Group by first column (Category)
                    ConsolidationFunction.Sum,
                    new int[] { 1 }, // Subtotal on second column (Value)
                    true,
                    true,
                    true);

                // Rufen Sie das SubtotalSetting vom Arbeitsblatt ab.
                SubtotalSetting subtotalSetting = worksheet.Cells.RetrieveSubtotalSetting(area);

                // Zeigen Sie die Eigenschaften des SubtotalSetting an.
                Console.WriteLine("Subtotal Setting Properties:");
                Console.WriteLine($"GroupBy field index: {subtotalSetting.GroupBy}");
                Console.WriteLine($"Subtotal Function: {subtotalSetting.SubtotalFunction}");
                Console.WriteLine($"TotalList contains column index: {subtotalSetting.TotalList[0]}");
                Console.WriteLine($"Summary Below Data: {subtotalSetting.SummaryBelowData}");

                // Speichere die Arbeitsmappe
                workbook.Save("SubtotalSettingDemo.xlsx");
                Console.WriteLine("SubtotalSetting demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SubtotalSetting: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


