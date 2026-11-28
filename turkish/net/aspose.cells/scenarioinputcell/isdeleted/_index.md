---
title: "ScenarioInputCell.IsDeleted"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ScenarioInputCell özelliği. Giriş hücresinin silinip silinmediğini gösterir"
type: docs
url: /tr/net/aspose.cells/scenarioinputcell/isdeleted/
---
## ScenarioInputCell.IsDeleted property

Giriş hücresinin silinip silinmediğini gösterir.

```csharp
public bool IsDeleted { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyIsDeletedDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir senaryo ekle
            int scenarioIndex = worksheet.Scenarios.Add("TestScenario");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Giriş hücrelerini ekle
            ScenarioInputCellCollection inputCells = scenario.InputCells;
            inputCells.Add(0, 0, "100");
            inputCells.Add(1, 1, "200");

            // Giriş hücrelerine eriş ve görüntüle
            ScenarioInputCell cell1 = inputCells[0];
            Console.WriteLine($"Cell A1 - Value: {cell1.Value}, IsDeleted: {cell1.IsDeleted}");

            // İlk giriş hücresini sil
            cell1.IsDeleted = true;
            Console.WriteLine($"After deletion - Cell A1 IsDeleted: {cell1.IsDeleted}");

            // Çalışma kitabını kaydedin
            workbook.Save("ScenarioWithDeletedCell.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


