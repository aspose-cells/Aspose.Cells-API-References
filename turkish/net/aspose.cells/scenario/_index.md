---
title: "Sınıf Scenario"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Scenario sınıfı. Tek bir senaryoyu temsil eder."
type: docs
url: /tr/net/aspose.cells/scenario/
---
## Scenario class

Bireysel bir senaryoyu temsil eder.

```csharp
public class Scenario
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Comment](../../aspose.cells/scenario/comment/) { get; set; } | Senaryonun yorumunu alır ve ayarlar. |
| [InputCells](../../aspose.cells/scenario/inputcells/) { get; } | Senaryonun giriş hücrelerini alır. |
| [IsHidden](../../aspose.cells/scenario/ishidden/) { get; set; } | Senaryonun gizli olup olmadığını gösterir. |
| [IsLocked](../../aspose.cells/scenario/islocked/) { get; set; } | Sayfa korunduğunda senaryonun düzenleme için kilitli olup olmadığını gösterir. |
| [Name](../../aspose.cells/scenario/name/) { get; set; } | Senaryonun adını alır ve ayarlar. |
| [User](../../aspose.cells/scenario/user/) { get; } | Senaryoyu en son değiştiren kullanıcının adını alır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ScenarioDemo
    {
        public static void ScenarioExample()
        {
            // Yeni bir çalışma kitabı oluştur ve ilk çalışma sayfasına eriş.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasının senaryo koleksiyonuna eriş.
            ScenarioCollection scenarios = worksheet.Scenarios;

            // Koleksiyona yeni bir senaryo ekleyin
            int scenarioIndex = scenarios.Add("MyScenario");
            Scenario scenario = scenarios[scenarioIndex];

            // Senaryonun özelliklerini ayarlama.
            scenario.Comment = "This is a test scenario.";
            scenario.Name = "TestScenario";
            scenario.IsHidden = false;
            scenario.IsLocked = true;

            // Sadece okunabilir özelliklere erişme.
            string user = scenario.User;
            ScenarioInputCellCollection inputCells = scenario.InputCells;

            // Çalışma kitabını kaydedin
            workbook.Save("ScenarioExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


