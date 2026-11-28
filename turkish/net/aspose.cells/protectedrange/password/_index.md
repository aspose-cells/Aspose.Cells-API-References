---
title: "ProtectedRange.Password"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ProtectedRange özelliği. Aralığı korumak için şifreyi temsil eder"
type: docs
url: /tr/net/aspose.cells/protectedrange/password/
---
## ProtectedRange.Password property

Aralığı korumak için kullanılan şifreyi temsil eder.

```csharp
public string Password { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangePropertyPasswordDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Korunan aralıklar koleksiyonu oluştur
            ProtectedRangeCollection allowRanges = worksheet.AllowEditRanges;

            // Bir korunan aralık ekle
            int index = allowRanges.Add("MyProtectedRange", 0, 0, 2, 2);
            ProtectedRange protectedRange = allowRanges[index];

            // Korunan aralık için şifre ayarla
            protectedRange.Password = "12345";

            // Çalışma kitabını kaydedin
            workbook.Save("ProtectedRangeWithPassword.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


