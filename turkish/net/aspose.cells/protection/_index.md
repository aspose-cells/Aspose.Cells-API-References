---
title: "Sınıf Protection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Protection sınıfı. Bir çalışma sayfası için mevcut çeşitli koruma seçeneklerini temsil eder"
type: docs
url: /tr/net/aspose.cells/protection/
---
## Protection class

Bir çalışma sayfası için mevcut çeşitli koruma seçeneklerini temsil eder.

```csharp
public class Protection
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AllowDeletingColumn](../../aspose.cells/protection/allowdeletingcolumn/) { get; set; } | Korunan bir çalışma sayfasında sütunların silinmesinin izin verilip verilmediğini temsil eder. |
| [AllowDeletingRow](../../aspose.cells/protection/allowdeletingrow/) { get; set; } | Korunan bir çalışma sayfasında satırların silinmesinin izin verilip verilmediğini temsil eder. |
| [AllowEditingContent](../../aspose.cells/protection/alloweditingcontent/) { get; set; } | Korunan bir çalışma sayfasında kilitli hücrelerin içeriğini düzenleme izni olup olmadığını temsil eder. |
| [AllowEditingObject](../../aspose.cells/protection/alloweditingobject/) { get; set; } | Korunan bir çalışma sayfasında çizim nesnelerini manipüle etme izni olup olmadığını temsil eder. |
| [AllowEditingScenario](../../aspose.cells/protection/alloweditingscenario/) { get; set; } | Korunan bir çalışma sayfasında senaryoları düzenleme izni olup olmadığını temsil eder. |
| [AllowFiltering](../../aspose.cells/protection/allowfiltering/) { get; set; } | Korunan bir çalışma sayfası korunmadan önce oluşturulan bir Otomatik Filtreyi kullanma izni olup olmadığını temsil eder. |
| [AllowFormattingCell](../../aspose.cells/protection/allowformattingcell/) { get; set; } | Korunan bir çalışma sayfasında hücre biçimlendirmesinin izin verilip verilmediğini temsil eder. |
| [AllowFormattingColumn](../../aspose.cells/protection/allowformattingcolumn/) { get; set; } | Korunan bir çalışma sayfasında sütun biçimlendirmesinin izin verilip verilmediğini temsil eder |
| [AllowFormattingRow](../../aspose.cells/protection/allowformattingrow/) { get; set; } | Korunan bir çalışma sayfasında satır biçimlendirmesinin izin verilip verilmediğini temsil eder |
| [AllowInsertingColumn](../../aspose.cells/protection/allowinsertingcolumn/) { get; set; } | Korunan bir çalışma sayfasında sütun eklemenin izin verilip verilmediğini temsil eder |
| [AllowInsertingHyperlink](../../aspose.cells/protection/allowinsertinghyperlink/) { get; set; } | Korunan bir çalışma sayfasında köprü eklemenin izin verilip verilmediğini temsil eder |
| [AllowInsertingRow](../../aspose.cells/protection/allowinsertingrow/) { get; set; } | Korunan bir çalışma sayfasında satır eklemenin izin verilip verilmediğini temsil eder |
| [AllowSelectingLockedCell](../../aspose.cells/protection/allowselectinglockedcell/) { get; set; } | Korunan bir çalışma sayfasında kilitli hücreleri seçme izni olup olmadığını temsil eder. |
| [AllowSelectingUnlockedCell](../../aspose.cells/protection/allowselectingunlockedcell/) { get; set; } | Korunan bir çalışma sayfasında kilidi kaldırılmış hücreleri seçme izni olup olmadığını temsil eder. |
| [AllowSorting](../../aspose.cells/protection/allowsorting/) { get; set; } | Korunan bir çalışma sayfasında sıralama seçeneğinin izin verilip verilmediğini temsil eder. |
| [AllowUsingPivotTable](../../aspose.cells/protection/allowusingpivottable/) { get; set; } | Korunan bir çalışma sayfasında özet tabloyu manipüle etme izni olup olmadığını temsil eder. |
| [IsProtectedWithPassword](../../aspose.cells/protection/isprotectedwithpassword/) { get; } | Çalışma sayfasının şifre ile korunup korunmadığını gösterir. |
| [Password](../../aspose.cells/protection/password/) { get; set; } | Çalışma sayfasını korumak için kullanılan şifreyi temsil eder. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Copy](../../aspose.cells/protection/copy/)(Protection) | Koruma bilgilerini kopyala. |
| [GetPasswordHash](../../aspose.cells/protection/getpasswordhash/)() | Mevcut şifrenin hash değerini alır. |
| [VerifyPassword](../../aspose.cells/protection/verifypassword/)(string) | Şifreyi doğrular. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ProtectionDemo
    {
        public static void ProtectionExample()
        {
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasının koruma ayarlarına erişim
            Protection protection = worksheet.Protection;

            // Çeşitli koruma özelliklerini ayarlama
            protection.AllowDeletingColumn = true;
            protection.AllowDeletingRow = true;
            protection.AllowFiltering = true;
            protection.AllowFormattingCell = true;
            protection.AllowFormattingColumn = true;
            protection.AllowFormattingRow = true;
            protection.AllowInsertingColumn = true;
            protection.AllowInsertingHyperlink = true;
            protection.AllowInsertingRow = true;
            protection.AllowSorting = true;
            protection.AllowUsingPivotTable = true;
            protection.AllowEditingContent = true;
            protection.AllowEditingObject = true;
            protection.AllowEditingScenario = true;
            protection.Password = "password123";
            protection.AllowSelectingLockedCell = true;
            protection.AllowSelectingUnlockedCell = true;

            // Çalışma sayfasının şifreyle korunup korunmadığını kontrol etme
            bool isProtectedWithPassword = protection.IsProtectedWithPassword;

            // Çalışma kitabını kaydetme
            workbook.Save("ProtectionExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


