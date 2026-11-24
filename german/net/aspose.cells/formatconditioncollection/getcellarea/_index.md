---
title: "FormatConditionCollection.GetCellArea"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormatConditionCollection-Methode. Gibt den bedingt formatierten Zellbereich nach Index zurück"
type: docs
url: /de/net/aspose.cells/formatconditioncollection/getcellarea/
---
## FormatConditionCollection.GetCellArea method

Gibt den bedingt formatierten Zellbereich nach Index zurück.

```csharp
public CellArea GetCellArea(int index)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | Int32 | der Index des bedingt formatierten Zellbereichs. |

### Rückgabewert

der bedingt formatierte Zellbereich

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodGetCellAreaWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].Value = i + j;
                }
            }

            // Bedingte Formatierung hinzufügen
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // Den Bereich der bedingten Formatierung festlegen
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 7;
            area.EndColumn = 3;
            fcc.AddArea(area);

            // Bedingung hinzufügen und Stil festlegen
            int conditionIndex = fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "5", "10");
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            fcc[conditionIndex].Style = style;

            // Zellbereichsinformationen abrufen und anzeigen
            CellArea retrievedArea = fcc.GetCellArea(0);
            Console.WriteLine("Conditional Format Area:");
            Console.WriteLine($"StartRow: {retrievedArea.StartRow}");
            Console.WriteLine($"StartColumn: {retrievedArea.StartColumn}");
            Console.WriteLine($"EndRow: {retrievedArea.EndRow}");
            Console.WriteLine($"EndColumn: {retrievedArea.EndColumn}");

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../cellarea/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


