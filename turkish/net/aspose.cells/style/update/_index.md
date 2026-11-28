---
title: "Style.Update"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style yöntemi. Adlandırılmış stili, bu adı verilen stili kullanan hücrelerin stillerine uygular. Stil üzerinde değişiklikleri tamamladıktan sonra Tamam düğmesine tıklamaya benzer. Yalnızca adlandırılmış stil için geçerlidir."
type: docs
url: /tr/net/aspose.cells/style/update/
---
## Style.Update method

Adlandırılmış stili, bu adlandırılmış stili kullanan hücrelerin stillerine uygula. Stil üzerinde değişiklikleri tamamladıktan sonra "ok" düğmesine tıklamaya benzer şekilde çalışır. Yalnızca adlandırılmış stil için geçerlidir.

```csharp
public void Update()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodUpdateDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir stil oluştur
            Style style = workbook.CreateStyle();
            style.Number = 3; // Set to Percent format
            
            // Stili A1 hücresine uygula
            worksheet.Cells["A1"].SetStyle(style);
            
            // Stili değiştir
            style.Number = 4; // Change to Currency format
            
            // Stil değişikliklerini güncelle
            style.Update();
            
            // Stilin güncellendiğini doğrula
            Console.WriteLine("Cell A1 Number Format: " + worksheet.Cells["A1"].GetStyle().Number);
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


