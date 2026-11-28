---
title: "Worksheet.Scenarios"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Scenario koleksiyonunu alır"
type: docs
url: /tr/net/aspose.cells/worksheet/scenarios/
---
## Worksheet.Scenarios property

[`Scenario`](../../scenario/) koleksiyonunu alır.

```csharp
public ScenarioCollection Scenarios { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyScenariosDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelere bazı veriler ekleyin
            worksheet.Cells["A1"].PutValue("Initial Value");
            worksheet.Cells["A2"].PutValue(100);
            
            // Senaryoları ekle
            ScenarioCollection scenarios = worksheet.Scenarios;
            int scenarioIndex1 = scenarios.Add("Scenario1");
            Scenario scenario1 = scenarios[scenarioIndex1];
            scenario1.Comment = "First test scenario";
            
            int scenarioIndex2 = scenarios.Add("Scenario2");
            Scenario scenario2 = scenarios[scenarioIndex2];
            scenario2.Comment = "Second test scenario";
            
            // Çalışma kitabını kaydedin
            workbook.Save("WorksheetPropertyScenariosDemo.xlsx");
            
            // Senaryoları temizle ve tekrar kaydet
            scenarios.Clear();
            workbook.Save("WorksheetPropertyScenariosDemo_Cleared.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ScenarioCollection](../../scenariocollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


