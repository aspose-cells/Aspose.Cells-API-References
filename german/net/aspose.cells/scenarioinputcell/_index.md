---
title: "Klasse ScenarioInputCell."
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ScenarioInputCell Klasse. Stellt die Eingabezelle für das Szenario dar."
type: docs
url: /de/net/aspose.cells/scenarioinputcell/
---
## ScenarioInputCell class

Stellt die Eingabezelle für das Szenario dar.

```csharp
public class ScenarioInputCell
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Column](../../aspose.cells/scenarioinputcell/column/) { get; } | Liest und setzt den Spaltenindex der Eingabezelle. |
| [IsDeleted](../../aspose.cells/scenarioinputcell/isdeleted/) { get; set; } | Gibt an, ob die Eingabezelle gelöscht ist. |
| [Name](../../aspose.cells/scenarioinputcell/name/) { get; } | Liest und setzt die Adresse der Eingabezelle. |
| [Row](../../aspose.cells/scenarioinputcell/row/) { get; } | Liest und setzt den Zeilenindex der Eingabezelle. |
| [Value](../../aspose.cells/scenarioinputcell/value/) { get; set; } | Liest und setzt den Wert der Eingabezelle. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ScenarioInputCellDemo
    {
        public static void ScenarioInputCellExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Szenario dem Arbeitsblatt hinzu.
            int scenarioIndex = worksheet.Scenarios.Add("Scenario 1");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Füge Eingabezellen dem Szenario hinzu.
            ScenarioInputCellCollection inputCells = scenario.InputCells;
            inputCells.Add(0, 0, "100"); // Adding cell A1 with value 100
            inputCells.Add(1, 1, "200"); // Adding cell B2 with value 200

            // Zugriff auf die Eingabezellen.
            ScenarioInputCell inputCell1 = inputCells[0];
            ScenarioInputCell inputCell2 = inputCells[1];

            // Anzeige der Eigenschaften der Eingabezellen.
            Console.WriteLine($"Input Cell 1: Row = {inputCell1.Row}, Column = {inputCell1.Column}, Value = {inputCell1.Value}, IsDeleted = {inputCell1.IsDeleted}");
            Console.WriteLine($"Input Cell 2: Row = {inputCell2.Row}, Column = {inputCell2.Column}, Value = {inputCell2.Value}, IsDeleted = {inputCell2.IsDeleted}");

            // Den Wert der ersten Eingabezelle ändern
            inputCell1.Value = "150";

            // Speichere die Arbeitsmappe
            workbook.Save("ScenarioInputCellExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


