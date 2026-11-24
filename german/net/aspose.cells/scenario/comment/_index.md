---
title: "Scenario.Comment"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Scenario-Eigenschaft. Gibt den Kommentar des Szenarios zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells/scenario/comment/
---
## Scenario.Comment property

Liest und setzt den Kommentar des Szenarios.

```csharp
public string Comment { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioPropertyCommentDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine Szenario-Sammlung
            ScenarioCollection scenarios = worksheet.Scenarios;
            
            // Ein Szenario hinzufügen
            int index = scenarios.Add("test");
            Scenario scenario = scenarios[index];
            
            // Setze Szenario-Eigenschaften
            scenario.IsLocked = true;
            scenario.Comment = "创建者 Simon 日期 " + DateTime.Now.ToShortDateString();
            
            // Füge Eingabezellen zum Szenario hinzu, indem du Zellreferenzen und Werte verwendest
            scenario.InputCells.Add(0, 6, "1");  // G16 (row 0, column 6)
            scenario.InputCells.Add(0, 0, "100"); // A1
            scenario.InputCells.Add(1, 1, "200"); // B2
            scenario.InputCells.Add(2, 2, "300"); // C3

            // Zeige den Kommentar des Szenarios an
            Console.WriteLine("Scenario Comment: " + scenario.Comment);
            
            // Speichere die Arbeitsmappe
            workbook.Save("ScenarioCommentDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


