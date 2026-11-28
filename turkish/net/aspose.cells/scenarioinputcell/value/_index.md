---
title: "ScenarioInputCell.Value"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ScenarioInputCell özelliği. Giriş hücresinin değerini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/scenarioinputcell/value/
---
## ScenarioInputCell.Value property

Giriş hücresinin değerini alır ve ayarlar.

```csharp
public string Value { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyValueDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir senaryo ekle
            int scenarioIndex = worksheet.Scenarios.Add("TestScenario");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Değerlerle giriş hücreleri ekle
            scenario.InputCells.Add(0, 0, "100"); // Cell A1
            scenario.InputCells.Add(1, 1, "200"); // Cell B2

            // Değerlere eriş ve değiştir
            ScenarioInputCell cell1 = scenario.InputCells[0];
            Console.WriteLine($"Original value: {cell1.Value}");
            cell1.Value = "150"; // Modify the value
            Console.WriteLine($"Modified value: {cell1.Value}");

            // Çalışma kitabını kaydedin
            workbook.Save("ScenarioValueDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


