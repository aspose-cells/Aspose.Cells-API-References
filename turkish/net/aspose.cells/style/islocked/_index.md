---
title: "Style.IsLocked"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style özelliği. Bir hücrenin değiştirilebilir olup olmadığını gösteren bir değeri alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/style/islocked/
---
## Style.IsLocked property

Bir hücrenin değiştirilebilir olup olmadığını gösteren bir değeri alır veya ayarlar.

```csharp
public bool IsLocked { get; set; }
```

### Açıklamalar

Hücreleri kilitlemek, çalışma sayfası korunmadıkça etkili değildir.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsLockedDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Bir hücre için IsLocked özelliğini ayarlayın
            Cell cell = cells["A1"];
            Style style = cell.GetStyle();
            style.IsLocked = true;
            cell.SetStyle(style);

            // Kilitlemeyi zorlamak için çalışma sayfasını koruyun
            worksheet.Protect(ProtectionType.All);

            // IsLocked durumunu doğrulayın ve yazdırın
            Console.WriteLine("Cell A1 IsLocked: " + cells["A1"].GetStyle().IsLocked);
            Console.WriteLine("Cell B1 IsLocked: " + cells["B1"].GetStyle().IsLocked);

            // Çalışma kitabını kaydedin
            workbook.Save("IsLockedDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


