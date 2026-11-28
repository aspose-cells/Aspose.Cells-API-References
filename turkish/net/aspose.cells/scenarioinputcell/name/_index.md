---
title: "ScenarioInputCell.Name"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ScenarioInputCell özelliği. Giriş hücresinin adresini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/scenarioinputcell/name/
---
## ScenarioInputCell.Name property

Giriş hücresinin adresini alır ve ayarlar.

```csharp
public string Name { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir senaryo oluştur
            ScenarioCollection scenarios = worksheet.Scenarios;
            int scenarioIndex = scenarios.Add("TestScenario");

            // Senaryoyu al
            Scenario scenario = scenarios[scenarioIndex];

            // Senaryoya giriş hücreleri ekle
            ScenarioInputCellCollection inputCells = scenario.InputCells;
            inputCells.Add(6, 15, "1"); // G16 is row 6, column 15 (0-based)
            inputCells.Add(7, 15, "2"); // H16 is row 7, column 15 (0-based)

            // Giriş hücrelerini al
            ScenarioInputCell inputCell1 = inputCells[0];
            ScenarioInputCell inputCell2 = inputCells[1];

            // Name özelliğinin kullanımını göster
            Console.WriteLine("First input cell name: " + inputCell1.Name);
            Console.WriteLine("Second input cell name: " + inputCell2.Name);

            // İsimlerin beklenen değerlerle eşleştiğini doğrula
            if (inputCell1.Name != "G16" || inputCell2.Name != "H16")
            {
                throw new Exception("Input cell names don't match expected values");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


