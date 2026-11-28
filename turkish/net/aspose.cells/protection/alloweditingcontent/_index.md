---
title: "Protection.AllowEditingContent"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Protection özelliği. Kullanıcının korunan bir çalışma sayfasında kilitli hücrelerin içeriğini düzenlemesine izin verilip verilmediğini gösterir"
type: docs
url: /tr/net/aspose.cells/protection/alloweditingcontent/
---
## Protection.AllowEditingContent property

Korunan bir çalışma sayfasında kilitli hücrelerin içeriğini düzenleme izni olup olmadığını temsil eder.

```csharp
public bool AllowEditingContent { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowEditingContentDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasını bir şifreyle koru
            worksheet.Protect(ProtectionType.All, "password", null);
            
            // AllowEditingContent özelliğini kontrol et ve göster
            Console.WriteLine("AllowEditingContent before setting: " + worksheet.Protection.AllowEditingContent);
            
            // AllowEditingContent özelliğini değiştir
            worksheet.Protection.AllowEditingContent = true;
            
            // Güncellenen özelliği kontrol et ve göster
            Console.WriteLine("AllowEditingContent after setting: " + worksheet.Protection.AllowEditingContent);
            
            // Çalışma kitabını kaydedin
            workbook.Save("ProtectionPropertyAllowEditingContentDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


