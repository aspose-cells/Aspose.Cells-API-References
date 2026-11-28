---
title: "Scenario.Comment"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Scenario özelliği. Senaryonun yorumunu alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/scenario/comment/
---
## Scenario.Comment property

Senaryonun yorumunu alır ve ayarlar.

```csharp
public string Comment { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioPropertyCommentDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir senaryo koleksiyonu oluşturun
            ScenarioCollection scenarios = worksheet.Scenarios;
            
            // Bir senaryo ekle
            int index = scenarios.Add("test");
            Scenario scenario = scenarios[index];
            
            // Senaryo özelliklerini ayarlayın
            scenario.IsLocked = true;
            scenario.Comment = "创建者 Simon 日期 " + DateTime.Now.ToShortDateString();
            
            // Senaryoya hücre referansları ve değerleri kullanarak giriş hücreleri ekle
            scenario.InputCells.Add(0, 6, "1");  // G16 (row 0, column 6)
            scenario.InputCells.Add(0, 0, "100"); // A1
            scenario.InputCells.Add(1, 1, "200"); // B2
            scenario.InputCells.Add(2, 2, "300"); // C3

            // Senaryo yorumunu göster
            Console.WriteLine("Scenario Comment: " + scenario.Comment);
            
            // Çalışma kitabını kaydedin
            workbook.Save("ScenarioCommentDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


