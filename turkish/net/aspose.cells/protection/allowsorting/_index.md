---
title: "Protection.AllowSorting"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Protection özelliği. Korumalı bir çalışma sayfasında sıralama seçeneğinin izinli olup olmadığını temsil eder."
type: docs
url: /tr/net/aspose.cells/protection/allowsorting/
---
## Protection.AllowSorting property

Korunan bir çalışma sayfasında sıralama seçeneğinin izin verilip verilmediğini temsil eder.

```csharp
public bool AllowSorting { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowSortingDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfası korumasını etkinleştir
            worksheet.Protect(ProtectionType.All);
            
            // AllowSorting dahil koruma özelliklerini ayarla
            Protection protection = worksheet.Protection;
            protection.AllowSorting = true;
            protection.AllowFiltering = true;
            protection.AllowEditingContent = false;

            // Koruma ayarlarını çıktıla
            Console.WriteLine("Protection Settings:");
            Console.WriteLine($"AllowSorting: {protection.AllowSorting}");
            Console.WriteLine($"AllowFiltering: {protection.AllowFiltering}");
            Console.WriteLine($"AllowEditingContent: {protection.AllowEditingContent}");

            // Sıralama yeteneğini göster
            if (protection.AllowSorting)
            {
                Console.WriteLine("\nSorting is allowed on this protected worksheet");
            }
            else
            {
                Console.WriteLine("\nSorting is not allowed on this protected worksheet");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


