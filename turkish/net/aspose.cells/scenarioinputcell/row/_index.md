---
title: "ScenarioInputCell.Row"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ScenarioInputCell özelliği. Giriş hücresinin satır indeksini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/scenarioinputcell/row/
---
## ScenarioInputCell.Row property

Giriş hücresinin satır indeksini alır ve ayarlar.

```csharp
public int Row { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyRowDemo
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

            // Row özelliğine eriş ve göster
            ScenarioInputCell cell1 = scenario.InputCells[0];
            Console.WriteLine($"First input cell is at row: {cell1.Row}");

            // Mevcut olanı değiştirmeye çalışmak yerine satır 2'de yeni bir hücre ekle
            worksheet.Cells[2, 0].Value = "30"; // Cell A3
            scenario.InputCells.Add(2, 0, "30");
            Console.WriteLine($"New input cell added at row: {scenario.InputCells[2].Row}");

            // Çalışma kitabını kaydedin
            workbook.Save("ScenarioInputCellRowDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


