---
title: "Klass ScenarioInputCell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ScenarioInputCell-klass. Representerar indatacell för scenariot"
type: docs
url: /sv/net/aspose.cells/scenarioinputcell/
---
## ScenarioInputCell class

Representerar inmatningscellen för scenariot.

```csharp
public class ScenarioInputCell
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Column](../../aspose.cells/scenarioinputcell/column/) { get; } | Hämtar och anger kolumnindex för indatacellen. |
| [IsDeleted](../../aspose.cells/scenarioinputcell/isdeleted/) { get; set; } | Anger om indatacellen är borttagen. |
| [Name](../../aspose.cells/scenarioinputcell/name/) { get; } | Hämtar och anger adressen för indatacellen. |
| [Row](../../aspose.cells/scenarioinputcell/row/) { get; } | Hämtar och anger radindex för indatacellen. |
| [Value](../../aspose.cells/scenarioinputcell/value/) { get; set; } | Hämtar och anger värdet för indatacellen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ScenarioInputCellDemo
    {
        public static void ScenarioInputCellExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till ett scenario i kalkylbladet
            int scenarioIndex = worksheet.Scenarios.Add("Scenario 1");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Lägg till indataceller till scenariot
            ScenarioInputCellCollection inputCells = scenario.InputCells;
            inputCells.Add(0, 0, "100"); // Adding cell A1 with value 100
            inputCells.Add(1, 1, "200"); // Adding cell B2 with value 200

            // Åtkomst till indatacellerna
            ScenarioInputCell inputCell1 = inputCells[0];
            ScenarioInputCell inputCell2 = inputCells[1];

            // Visar egenskaper för indatacellerna
            Console.WriteLine($"Input Cell 1: Row = {inputCell1.Row}, Column = {inputCell1.Column}, Value = {inputCell1.Value}, IsDeleted = {inputCell1.IsDeleted}");
            Console.WriteLine($"Input Cell 2: Row = {inputCell2.Row}, Column = {inputCell2.Column}, Value = {inputCell2.Value}, IsDeleted = {inputCell2.IsDeleted}");

            // Ändra värdet för den första indatacellen
            inputCell1.Value = "150";

            // Spara arbetsboken
            workbook.Save("ScenarioInputCellExample.xlsx");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


