---
title: "Scenario.InputCells"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Scenario özelliği. Senaryonun giriş hücrelerini alır"
type: docs
url: /tr/net/aspose.cells/scenario/inputcells/
---
## Scenario.InputCells property

Senaryonun giriş hücrelerini alır.

```csharp
public ScenarioInputCellCollection InputCells { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioPropertyInputCellsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir senaryo ekle
            int scenarioIndex = worksheet.Scenarios.Add("Scenario 1");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // InputCells özelliğini kullanarak senaryoya giriş hücreleri ekleyin
            ScenarioInputCellCollection inputCells = scenario.InputCells;
            inputCells.Add(0, 0, "100"); // Cell A1
            inputCells.Add(1, 1, "200"); // Cell B2

            // İlk giriş hücresinin değerini değiştirin
            inputCells[0].Value = "150";

            // Çalışma kitabını kaydedin
            workbook.Save("ScenarioInputCellsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ScenarioInputCellCollection](../../scenarioinputcellcollection/)
* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


