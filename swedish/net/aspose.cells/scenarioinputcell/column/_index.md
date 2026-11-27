---
title: "ScenarioInputCell.Column"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ScenarioInputCell‑egenskap. Hämtar och sätter kolumnindex för inmatningscellen"
type: docs
url: /sv/net/aspose.cells/scenarioinputcell/column/
---
## ScenarioInputCell.Column property

Hämtar och anger kolumnindex för indatacellen.

```csharp
public int Column { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyColumnDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till ett scenario i kalkylbladet
            int scenarioIndex = worksheet.Scenarios.Add("Scenario1");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Lägg till indataceller till scenariot
            scenario.InputCells.Add(0, 0, "10"); // Cell A1
            scenario.InputCells.Add(1, 1, "20"); // Cell B2

            // Åtkomst och demonstration av Column‑egenskapen
            ScenarioInputCell cell1 = scenario.InputCells[0];
            Console.WriteLine($"First input cell is at column: {cell1.Column}");

            // Eftersom Column är skrivskyddad måste vi ta bort och lägga till igen för att ändra kolumnen
            string value = cell1.Value;
            scenario.InputCells.RemoveAt(0);
            scenario.InputCells.Add(0, 2, value); // Add at new column 2 with same value

            // Verifiera ändringen
            cell1 = scenario.InputCells[0];
            Console.WriteLine($"Modified first input cell column to: {cell1.Column}");

            // Spara arbetsboken
            workbook.Save("ScenarioInputCellColumnDemo.xlsx");
        }
    }
}
```

### Se även

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


