---
title: "ScenarioInputCell.Column"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ScenarioInputCell özelliği. Giriş hücresinin sütun indeksini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/scenarioinputcell/column/
---
## ScenarioInputCell.Column property

Giriş hücresinin sütun indeksini alır ve ayarlar.

```csharp
public int Column { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyColumnDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir senaryo ekle
            int scenarioIndex = worksheet.Scenarios.Add("Scenario1");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Senaryoya giriş hücreleri ekle
            scenario.InputCells.Add(0, 0, "10"); // Cell A1
            scenario.InputCells.Add(1, 1, "20"); // Cell B2

            // Column özelliğine eriş ve göster
            ScenarioInputCell cell1 = scenario.InputCells[0];
            Console.WriteLine($"First input cell is at column: {cell1.Column}");

            // Column yalnızca okunabilir olduğundan, sütunu değiştirmek için kaldırıp yeniden eklememiz gerekir
            string value = cell1.Value;
            scenario.InputCells.RemoveAt(0);
            scenario.InputCells.Add(0, 2, value); // Add at new column 2 with same value

            // Değişikliği doğrulayın
            cell1 = scenario.InputCells[0];
            Console.WriteLine($"Modified first input cell column to: {cell1.Column}");

            // Çalışma kitabını kaydedin
            workbook.Save("ScenarioInputCellColumnDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


