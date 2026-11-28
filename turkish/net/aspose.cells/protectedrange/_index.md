---
title: "Sınıf ProtectedRange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ProtectedRange sınıfı. Sayfa koruması AÇIK olduğunda düzenlemeye izin verilen belirli bir aralık."
type: docs
url: /tr/net/aspose.cells/protectedrange/
---
## ProtectedRange class

Sayfa koruması AÇIK olduğunda düzenlemeye izin verilen belirtilen bir aralık.

```csharp
public class ProtectedRange
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CellArea](../../aspose.cells/protectedrange/cellarea/) { get; } | Korunacak hücre alanını temsil eden [`CellArea`](./cellarea/) nesnesini alır. |
| [IsProtectedWithPassword](../../aspose.cells/protectedrange/isprotectedwithpassword/) { get; } | Çalışma sayfasının şifre ile korunup korunmadığını gösterir. |
| [Name](../../aspose.cells/protectedrange/name/) { get; set; } | Aralık başlığını alır. Bu, adlandırılmış bir aralık tanımı yerine bir tanımlayıcı olarak kullanılır. |
| [Password](../../aspose.cells/protectedrange/password/) { get; set; } | Aralığı korumak için kullanılan şifreyi temsil eder. |
| [SecurityDescriptor](../../aspose.cells/protectedrange/securitydescriptor/) { get; set; } | Güvenlik tanımlayıcısı, aralığa erişmek için şifre girmeden bu aralığı düzenleyebilecek kullanıcı hesaplarını tanımlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [AddArea](../../aspose.cells/protectedrange/addarea/)(int, int, int, int) | Bu öğeye bir başvurulan alan ekler. |
| [GetAreas](../../aspose.cells/protectedrange/getareas/)() | Tüm başvurulan alanları alır. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassProtectedRangeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Korunan aralıkların koleksiyonunu al.
            ProtectedRangeCollection protectedRanges = worksheet.AllowEditRanges;
            
            // Yeni bir korunan aralık ekle (A1:J10)
            int index = protectedRanges.Add("MyProtectedRange", 0, 0, 10, 10);
            
            // Korunan aralığı al
            ProtectedRange protectedRange = protectedRanges[index];
            
            // Güvenlik tanımlayıcısını ayarla
            string securityDescriptor = "O:WDG:WDD:(D;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1000)(A;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1013)";
            protectedRange.SecurityDescriptor = securityDescriptor;
            
            // Çalışma kitabını kaydedin
            workbook.Save("ProtectedRangeDemo.xlsx");
            
            Console.WriteLine("Protected range demo completed successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


