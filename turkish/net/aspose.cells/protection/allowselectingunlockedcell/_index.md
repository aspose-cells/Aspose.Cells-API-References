---
title: "Protection.AllowSelectingUnlockedCell"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Protection özelliği. Kullanıcının korumalı bir çalışma sayfasında kilidi açılmış hücreleri seçmesine izin verilip verilmediğini temsil eder."
type: docs
url: /tr/net/aspose.cells/protection/allowselectingunlockedcell/
---
## Protection.AllowSelectingUnlockedCell property

Korunan bir çalışma sayfasında kilidi kaldırılmış hücreleri seçme izni olup olmadığını temsil eder.

```csharp
public bool AllowSelectingUnlockedCell { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowSelectingUnlockedCellDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasını tüm koruma seçenekleriyle koruyun.
            Protection protection = worksheet.Protection;
            
            // AllowSelectingUnlockedCell değerini true olarak ayarlayın.
            protection.AllowSelectingUnlockedCell = true;
            protection.AllowSelectingLockedCell = false;
            
            // Şifreyle koruma uygulayın.
            protection.Password = "password123";
            worksheet.Protect(ProtectionType.All);

            // Ayarı doğrula
            Console.WriteLine("AllowSelectingUnlockedCell: " + protection.AllowSelectingUnlockedCell);
            Console.WriteLine("Worksheet is protected: " + worksheet.IsProtected);

            // Çalışma kitabını kaydedin
            workbook.Save("ProtectionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


