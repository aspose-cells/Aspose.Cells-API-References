---
title: "ScenarioInputCellCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ScenarioInputCellCollection özelliği. Listede indeksle ScenarioInputCell alır"
type: docs
url: /tr/net/aspose.cells/scenarioinputcellcollection/item/
---
## ScenarioInputCellCollection indexer

Listede indeksle [`ScenarioInputCell`](../../scenarioinputcell/) alır.

```csharp
public ScenarioInputCell this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | Listede belirli indeks |

### Dönüş Değeri

[`ScenarioInputCell`](../../scenarioinputcell/) nesnesi

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int scenarioIndex = worksheet.Scenarios.Add("Scenario1");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];
            ScenarioInputCellCollection inputCells = scenario.InputCells;

            inputCells.Add(0, 0, "10");
            inputCells.Add(1, 1, "20");

            // Item özelliğinin kullanımını göster
            ScenarioInputCell firstCell = inputCells[0];
            ScenarioInputCell secondCell = inputCells[1];

            Console.WriteLine($"First cell - Row: {firstCell.Row}, Column: {firstCell.Column}, Value: {firstCell.Value}");
            Console.WriteLine($"Second cell - Row: {secondCell.Row}, Column: {secondCell.Column}, Value: {secondCell.Value}");

            workbook.Save("ScenarioInputCellCollectionExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ScenarioInputCell](../../scenarioinputcell/)
* class [ScenarioInputCellCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


