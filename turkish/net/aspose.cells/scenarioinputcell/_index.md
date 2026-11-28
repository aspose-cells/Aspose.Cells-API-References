---
title: "Sınıf ScenarioInputCell"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ScenarioInputCell sınıfı. Senaryo için giriş hücresini temsil eder"
type: docs
url: /tr/net/aspose.cells/scenarioinputcell/
---
## ScenarioInputCell class

Senaryo için giriş hücresini temsil eder.

```csharp
public class ScenarioInputCell
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Column](../../aspose.cells/scenarioinputcell/column/) { get; } | Giriş hücresinin sütun indeksini alır ve ayarlar. |
| [IsDeleted](../../aspose.cells/scenarioinputcell/isdeleted/) { get; set; } | Giriş hücresinin silinip silinmediğini gösterir. |
| [Name](../../aspose.cells/scenarioinputcell/name/) { get; } | Giriş hücresinin adresini alır ve ayarlar. |
| [Row](../../aspose.cells/scenarioinputcell/row/) { get; } | Giriş hücresinin satır indeksini alır ve ayarlar. |
| [Value](../../aspose.cells/scenarioinputcell/value/) { get; set; } | Giriş hücresinin değerini alır ve ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ScenarioInputCellDemo
    {
        public static void ScenarioInputCellExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir senaryo ekle
            int scenarioIndex = worksheet.Scenarios.Add("Scenario 1");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Senaryoya giriş hücreleri ekle
            ScenarioInputCellCollection inputCells = scenario.InputCells;
            inputCells.Add(0, 0, "100"); // Adding cell A1 with value 100
            inputCells.Add(1, 1, "200"); // Adding cell B2 with value 200

            // Giriş hücrelerine erişim
            ScenarioInputCell inputCell1 = inputCells[0];
            ScenarioInputCell inputCell2 = inputCells[1];

            // Giriş hücrelerinin özelliklerini gösterme
            Console.WriteLine($"Input Cell 1: Row = {inputCell1.Row}, Column = {inputCell1.Column}, Value = {inputCell1.Value}, IsDeleted = {inputCell1.IsDeleted}");
            Console.WriteLine($"Input Cell 2: Row = {inputCell2.Row}, Column = {inputCell2.Column}, Value = {inputCell2.Value}, IsDeleted = {inputCell2.IsDeleted}");

            // İlk giriş hücresinin değerini değiştir
            inputCell1.Value = "150";

            // Çalışma kitabını kaydedin
            workbook.Save("ScenarioInputCellExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


