---
title: "Worksheet.Scenarios"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Gibt die Sammlung von Scenario zurück"
type: docs
url: /de/net/aspose.cells/worksheet/scenarios/
---
## Worksheet.Scenarios property

Gibt die Sammlung von [`Scenario`](../../scenario/) zurück.

```csharp
public ScenarioCollection Scenarios { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyScenariosDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Einige Daten zu den Zellen hinzufügen
            worksheet.Cells["A1"].PutValue("Initial Value");
            worksheet.Cells["A2"].PutValue(100);
            
            // Szenarien hinzufügen
            ScenarioCollection scenarios = worksheet.Scenarios;
            int scenarioIndex1 = scenarios.Add("Scenario1");
            Scenario scenario1 = scenarios[scenarioIndex1];
            scenario1.Comment = "First test scenario";
            
            int scenarioIndex2 = scenarios.Add("Scenario2");
            Scenario scenario2 = scenarios[scenarioIndex2];
            scenario2.Comment = "Second test scenario";
            
            // Speichere die Arbeitsmappe
            workbook.Save("WorksheetPropertyScenariosDemo.xlsx");
            
            // Szenarien löschen und erneut speichern
            scenarios.Clear();
            workbook.Save("WorksheetPropertyScenariosDemo_Cleared.xlsx");
        }
    }
}
```

### Siehe auch

* class [ScenarioCollection](../../scenariocollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


