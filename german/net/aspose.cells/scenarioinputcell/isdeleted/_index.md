---
title: "ScenarioInputCell.IsDeleted"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ScenarioInputCell-Eigenschaft. Gibt an, ob die Eingabezelle gelöscht ist"
type: docs
url: /de/net/aspose.cells/scenarioinputcell/isdeleted/
---
## ScenarioInputCell.IsDeleted property

Gibt an, ob die Eingabezelle gelöscht ist.

```csharp
public bool IsDeleted { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyIsDeletedDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ein Szenario hinzufügen
            int scenarioIndex = worksheet.Scenarios.Add("TestScenario");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Eingabezellen hinzufügen
            ScenarioInputCellCollection inputCells = scenario.InputCells;
            inputCells.Add(0, 0, "100");
            inputCells.Add(1, 1, "200");

            // Eingabezellen zugreifen und anzeigen
            ScenarioInputCell cell1 = inputCells[0];
            Console.WriteLine($"Cell A1 - Value: {cell1.Value}, IsDeleted: {cell1.IsDeleted}");

            // Die erste Eingabezelle löschen
            cell1.IsDeleted = true;
            Console.WriteLine($"After deletion - Cell A1 IsDeleted: {cell1.IsDeleted}");

            // Speichere die Arbeitsmappe
            workbook.Save("ScenarioWithDeletedCell.xlsx");
        }
    }
}
```

### Siehe auch

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


