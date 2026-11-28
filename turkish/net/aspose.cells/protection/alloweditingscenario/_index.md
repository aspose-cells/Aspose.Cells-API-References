---
title: "Protection.AllowEditingScenario"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Protection özelliği. Kullanıcının korumalı bir çalışma sayfasında senaryoları düzenlemesine izin verilip verilmediğini temsil eder."
type: docs
url: /tr/net/aspose.cells/protection/alloweditingscenario/
---
## Protection.AllowEditingScenario property

Korunan bir çalışma sayfasında senaryoları düzenleme izni olup olmadığını temsil eder.

```csharp
public bool AllowEditingScenario { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowEditingScenarioDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(200);

            // Çalışma sayfası koruma ayarlarına erişin.
            Protection protection = worksheet.Protection;

            // AllowEditingScenario etkinleştirilmiş şekilde koruma özelliklerini ayarlayın.
            protection.AllowEditingScenario = true;
            protection.AllowFormattingCell = true;  // Corrected property name
            protection.Password = "password123";

            // Çalışma sayfasını koru
            worksheet.Protect(ProtectionType.All);

            // Çalışma kitabını kaydedin
            workbook.Save("ProtectionWithScenarioEditing.xlsx");

            Console.WriteLine("Worksheet protected with AllowEditingScenario enabled.");
        }
    }
}
```

### Ayrıca Bakınız

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


