---
title: "ScenarioCollection.LastSelected"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ScenarioCollection özelliği. Kullanıcı tarafından çalıştırılmak/gösterilmek üzere en son seçilen senaryoyu gösterir"
type: docs
url: /tr/net/aspose.cells/scenariocollection/lastselected/
---
## ScenarioCollection.LastSelected property

Kullanıcı tarafından çalıştırılmak/gösterilmek üzere son seçilen senaryoyu belirtir.

```csharp
public int LastSelected { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioCollectionPropertyLastSelectedDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Senaryoları ekle
            ScenarioCollection scenarios = worksheet.Scenarios;
            scenarios.Add("Scenario1");
            scenarios.Add("Scenario2");

            // Aktif senaryoyu ve en son seçilen indeksi ayarla
            scenarios.ActiveIndex = 1;
            scenarios.LastSelected = 1;

            // LastSelected özelliğini doğrula ve göster
            Console.WriteLine("Total scenarios: " + scenarios.Count);
            Console.WriteLine("Active scenario index: " + scenarios.ActiveIndex);
            Console.WriteLine("Last selected scenario index: " + scenarios.LastSelected);

            // En son seçilen indeksi değiştir
            scenarios.LastSelected = 0;
            Console.WriteLine("Updated last selected scenario index: " + scenarios.LastSelected);
        }
    }
}
```

### Ayrıca Bakınız

* class [ScenarioCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


