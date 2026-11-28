---
title: "Style.IsProtectionApplied"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style özelliği. Koruma biçimlendirmesinin uygulanıp uygulanmayacağını belirtir"
type: docs
url: /tr/net/aspose.cells/style/isprotectionapplied/
---
## Style.IsProtectionApplied property

Koruma biçimlendirmesinin uygulanıp uygulanmayacağını belirt.

```csharp
public bool IsProtectionApplied { get; set; }
```

### Açıklamalar

Yalnızca adlandırılmış stil için.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsProtectionAppliedDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir stil nesnesi oluşturun
            Style style = workbook.CreateStyle();
            
            // Koruma özelliklerini ayarla
            style.IsLocked = true;
            style.IsFormulaHidden = true;
            style.IsProtectionApplied = true;
            
            // Stili bir hücreye uygula
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            
            // Koruma ayarlarını doğrula
            Console.WriteLine("IsProtectionApplied: " + style.IsProtectionApplied);
            Console.WriteLine("IsLocked: " + style.IsLocked);
            Console.WriteLine("IsFormulaHidden: " + style.IsFormulaHidden);
            
            // Koruma ayarlarını değiştir
            style.IsProtectionApplied = false;
            Console.WriteLine("\nAfter changing IsProtectionApplied to false:");
            Console.WriteLine("IsProtectionApplied: " + style.IsProtectionApplied);
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


