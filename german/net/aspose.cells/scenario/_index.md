---
title: "Klasse Scenario"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Scenario‑Klasse. Stellt ein einzelnes Szenario dar"
type: docs
url: /de/net/aspose.cells/scenario/
---
## Scenario class

Stellt ein einzelnes Szenario dar.

```csharp
public class Scenario
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Comment](../../aspose.cells/scenario/comment/) { get; set; } | Liest und setzt den Kommentar des Szenarios. |
| [InputCells](../../aspose.cells/scenario/inputcells/) { get; } | Liest die Eingabezellen des Szenarios. |
| [IsHidden](../../aspose.cells/scenario/ishidden/) { get; set; } | Gibt an, ob das Szenario ausgeblendet ist. |
| [IsLocked](../../aspose.cells/scenario/islocked/) { get; set; } | Gibt an, ob das Szenario beim geschützten Blatt für die Bearbeitung gesperrt ist. |
| [Name](../../aspose.cells/scenario/name/) { get; set; } | Liest und setzt den Namen des Szenarios. |
| [User](../../aspose.cells/scenario/user/) { get; } | Liest den Namen des Benutzers, der das Szenario zuletzt geändert hat. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ScenarioDemo
    {
        public static void ScenarioExample()
        {
            // Erstelle eine neue Arbeitsmappe und greife auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Greife auf die Szenario‑Sammlung des Arbeitsblatts zu
            ScenarioCollection scenarios = worksheet.Scenarios;

            // Fügen Sie ein neues Szenario zur Sammlung hinzu
            int scenarioIndex = scenarios.Add("MyScenario");
            Scenario scenario = scenarios[scenarioIndex];

            // Einstellen von Eigenschaften des Szenarios
            scenario.Comment = "This is a test scenario.";
            scenario.Name = "TestScenario";
            scenario.IsHidden = false;
            scenario.IsLocked = true;

            // Zugriff auf schreibgeschützte Eigenschaften
            string user = scenario.User;
            ScenarioInputCellCollection inputCells = scenario.InputCells;

            // Speichere die Arbeitsmappe
            workbook.Save("ScenarioExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


