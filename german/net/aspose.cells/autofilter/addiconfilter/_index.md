---
title: "AutoFilter.AddIconFilter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AutoFilter‑Methode. Fügt einen Symbolfilter hinzu"
type: docs
url: /de/net/aspose.cells/autofilter/addiconfilter/
---
## AutoFilter.AddIconFilter method

Fügt einen Symbolfilter hinzu.

```csharp
public void AddIconFilter(int fieldIndex, IconSetType iconSetType, int iconId)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldIndex | Int32 | Der ganzzahlige Versatz des Feldes, auf dem der Filter basieren soll (vom linken Rand der Liste; das linkeste Feld ist Feld 0). |
| iconSetType | IconSetType | Der Symbolsatztyp. |
| iconId | Int32 | Die Symbol-ID. |

### Hinweise

Unterstützt nur das Hinzufügen des Symbolfilters. Unterstützt nicht die Prüfung, welche Zeile sichtbar ist, wenn der Filter ein Symbolfilter ist.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodAddIconFilterWithInt32IconSetTypeInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten in Spalte A befüllen.
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Values");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["A5"].PutValue(40);
            worksheet.Cells["A6"].PutValue(50);
            cell = worksheet.Cells["B1"];
            cell.PutValue("Values2");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);
            worksheet.Cells["B6"].PutValue(50);

            ConditionalFormattingCollection cfs = worksheet.ConditionalFormattings;
            FormatConditionCollection fcs = cfs[cfs.Add()];
            fcs.AddArea(CellArea.CreateCellArea(1, 0, 5, 1));
            FormatCondition fc = fcs[fcs.AddCondition(FormatConditionType.IconSet)];

            // Auto-Filter-Instanz abrufen
            AutoFilter autoFilter = worksheet.AutoFilter;
            
            // Auto-Filter-Bereich (A1:A6) mit startRow, startColumn, endRow festlegen
            autoFilter.SetRange(0, 0, 1);

            try
            {
                // Symbolfilter zur ersten Spalte hinzufügen (fieldIndex: 0)
                // Verwenden des 3-Signalampel-Symbolsets (IconSetType.TrafficLights31)
                // Filtern nach dem ersten Symbol im Set (iconId: 0)
                autoFilter.AddIconFilter(0, IconSetType.TrafficLights31, 0);
                
                // Filter aktualisieren, um Änderungen anzuwenden
                autoFilter.Refresh();

                Console.WriteLine("Added icon filter to column A showing items with first traffic light icon");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddIconFilter: {ex.Message}");
            }

            // Speichere die geänderte Arbeitsmappe
            workbook.Save("AutoFilterMethodAddIconFilterWithInt32IconSetTypeInt32Demo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [IconSetType](../../iconsettype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


