---
title: "Enum PasteOperationType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.PasteOperationType enum'ı. Bir aralık yapıştırılırken işlem türünü temsil eder"
type: docs
url: /tr/net/aspose.cells/pasteoperationtype/
---
## PasteOperationType enumeration

Bir aralık yapıştırılırken işlem türünü temsil eder.

```csharp
public enum PasteOperationType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | İşlem yok. |
| Add | `1` | Ekle |
| Subtract | `2` | Çıkar |
| Multiply | `3` | Çarp |
| Divide | `4` | Böl |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassPasteOperationTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Hücrelere örnek veri ekle
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["B1"].PutValue(20);
            sheet.Cells["C1"].PutValue(30);
            
            // PasteOperationType.None ile yapıştırma seçenekleri oluştur
            var pasteOptions = new PasteOptions()
            {
                PasteType = PasteType.Values,
                OperationType = PasteOperationType.None,
                SkipBlanks = false,
                Transpose = false
            };

            // Aralık oluştur ve yapıştırma seçenekleriyle kopyala
            Aspose.Cells.Range sourceRange = sheet.Cells.CreateRange("A1", "C1");
            Aspose.Cells.Range destRange = sheet.Cells.CreateRange("A2", "C2");
            sourceRange.Copy(destRange, pasteOptions);

            // Çalışma kitabını kaydedin
            workbook.Save("PasteOperationTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


