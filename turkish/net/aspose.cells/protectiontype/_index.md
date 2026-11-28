---
title: "Enum ProtectionType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ProtectionType enum. Çalışma kitabı/çalışma sayfası koruma türünü temsil eder"
type: docs
url: /tr/net/aspose.cells/protectiontype/
---
## ProtectionType enumeration

Çalışma kitabı/çalışma sayfası koruma türünü temsil eder.

```csharp
public enum ProtectionType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| All | `0` | Hepsini korumayı temsil eder. |
| Contents | `1` | İçeriği korumayı temsil eder, Çalışma sayfası korumasında kullanılır. |
| Objects | `2` | Nesneleri korumayı temsil eder, Çalışma sayfası korumasında kullanılır. |
| Scenarios | `3` | Senaryoları korumayı temsil eder, Çalışma sayfası korumasında kullanılır. |
| Structure | `4` | Yapıyı korumayı temsil eder, Çalışma kitabı korumasında kullanılır. |
| Windows | `5` | Pencereyi korumayı temsil eder, Çalışma kitabı korumasında kullanılır. |
| None | `6` | Koruma olmadığını temsil eder. Yalnızca Reading özelliği için. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassProtectionTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasını tüm koruma türleriyle koruyun
            worksheet.Protect(ProtectionType.All);
            
            // Koruma özelliklerine erişimi gösterin
            Console.WriteLine("Worksheet protection settings:");
            Console.WriteLine("AllowDeletingColumn: " + worksheet.Protection.AllowDeletingColumn);
            Console.WriteLine("AllowDeletingRow: " + worksheet.Protection.AllowDeletingRow);
            Console.WriteLine("AllowFiltering: " + worksheet.Protection.AllowFiltering);
            Console.WriteLine("AllowFormattingCell: " + worksheet.Protection.AllowFormattingCell);
            Console.WriteLine("AllowFormattingColumn: " + worksheet.Protection.AllowFormattingColumn);
            Console.WriteLine("AllowFormattingRow: " + worksheet.Protection.AllowFormattingRow);
            Console.WriteLine("AllowInsertingColumn: " + worksheet.Protection.AllowInsertingColumn);
            Console.WriteLine("AllowInsertingHyperlink: " + worksheet.Protection.AllowInsertingHyperlink);
            Console.WriteLine("AllowInsertingRow: " + worksheet.Protection.AllowInsertingRow);
            Console.WriteLine("AllowSorting: " + worksheet.Protection.AllowSorting);
            Console.WriteLine("AllowUsingPivotTable: " + worksheet.Protection.AllowUsingPivotTable);
            
            // Çalışma sayfasının korumasını kaldırın
            worksheet.Unprotect();
            
            // Belirli koruma türleriyle koruyun
            worksheet.Protect(ProtectionType.Contents | ProtectionType.Objects);
            Console.WriteLine("\nWorksheet protected with Contents and Objects only");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


