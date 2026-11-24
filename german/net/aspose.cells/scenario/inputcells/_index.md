---
title: "Scenario.InputCells"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Scenario-Eigenschaft. Gibt die Eingabezellen des Szenarios zurück"
type: docs
url: /de/net/aspose.cells/scenario/inputcells/
---
## Scenario.InputCells property

Liest die Eingabezellen des Szenarios.

```csharp
public ScenarioInputCellCollection InputCells { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioPropertyInputCellsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Szenario dem Arbeitsblatt hinzu.
            int scenarioIndex = worksheet.Scenarios.Add("Scenario 1");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Füge Eingabezellen zum Szenario hinzu, indem die InputCells‑Eigenschaft verwendet wird
            ScenarioInputCellCollection inputCells = scenario.InputCells;
            inputCells.Add(0, 0, "100"); // Cell A1
            inputCells.Add(1, 1, "200"); // Cell B2

            // Ändere den Wert der ersten Eingabezelle
            inputCells[0].Value = "150";

            // Speichere die Arbeitsmappe
            workbook.Save("ScenarioInputCellsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ScenarioInputCellCollection](../../scenarioinputcellcollection/)
* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


