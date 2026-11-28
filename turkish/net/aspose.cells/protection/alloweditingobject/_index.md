---
title: "Protection.AllowEditingObject"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Protection özelliği. Kullanıcının korumalı bir çalışma sayfasında çizim nesnelerini manipüle etmesine izin verilip verilmediğini temsil eder."
type: docs
url: /tr/net/aspose.cells/protection/alloweditingobject/
---
## Protection.AllowEditingObject property

Korunan bir çalışma sayfasında çizim nesnelerini manipüle etme izni olup olmadığını temsil eder.

```csharp
public bool AllowEditingObject { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowEditingObjectDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // AllowEditingObject etkinleştirilmiş şekilde koruma ayarlarını belirleyin.
            Protection protection = worksheet.Protection;
            protection.AllowEditingObject = true;
            protection.AllowEditingContent = false; // Contrast with AllowEditingObject
            worksheet.Protect(ProtectionType.All);

            // Korumayı işaretlerini kontrol edin.
            Console.WriteLine("Protection Settings:");
            Console.WriteLine($"AllowEditingObject: {protection.AllowEditingObject}");
            Console.WriteLine($"AllowEditingContent: {protection.AllowEditingContent}");

            // Düzenlemeyi test etmek için bir metin kutusu (nesne) oluşturun.
            worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            
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


