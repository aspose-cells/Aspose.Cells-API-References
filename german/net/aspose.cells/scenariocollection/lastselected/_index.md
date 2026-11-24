---
title: "ScenarioCollection.LastSelected"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ScenarioCollection-Eigenschaft. Gibt an, welches Szenario zuletzt vom Benutzer ausgewählt wurde, um ausgeführt/angezeigt zu werden"
type: docs
url: /de/net/aspose.cells/scenariocollection/lastselected/
---
## ScenarioCollection.LastSelected property

Gibt an, welches Szenario zuletzt vom Benutzer ausgewählt wurde, um ausgeführt/angezeigt zu werden.

```csharp
public int LastSelected { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioCollectionPropertyLastSelectedDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Szenarien hinzufügen
            ScenarioCollection scenarios = worksheet.Scenarios;
            scenarios.Add("Scenario1");
            scenarios.Add("Scenario2");

            // Legen Sie das aktive Szenario und den zuletzt ausgewählten Index fest
            scenarios.ActiveIndex = 1;
            scenarios.LastSelected = 1;

            // Überprüfen und demonstrieren Sie die LastSelected-Eigenschaft
            Console.WriteLine("Total scenarios: " + scenarios.Count);
            Console.WriteLine("Active scenario index: " + scenarios.ActiveIndex);
            Console.WriteLine("Last selected scenario index: " + scenarios.LastSelected);

            // Letzten ausgewählten Index ändern
            scenarios.LastSelected = 0;
            Console.WriteLine("Updated last selected scenario index: " + scenarios.LastSelected);
        }
    }
}
```

### Siehe auch

* class [ScenarioCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


