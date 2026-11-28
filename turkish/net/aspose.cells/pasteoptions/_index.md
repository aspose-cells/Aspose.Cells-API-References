---
title: "Sınıf PasteOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.PasteOptions sınıfı. Yapıştırma özel seçeneklerini temsil eder"
type: docs
url: /tr/net/aspose.cells/pasteoptions/
---
## PasteOptions class

Özel yapıştırma seçeneklerini temsil eder.

```csharp
public class PasteOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [PasteOptions](pasteoptions/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [IgnoreLinksToOriginalFile](../../aspose.cells/pasteoptions/ignorelinkstooriginalfile/) { get; set; } | Orijinal dosyaya bağlantıları yok say. |
| [KeepOldTables](../../aspose.cells/pasteoptions/keepoldtables/) { get; set; } | Tabloları hedef aralıkta tutar. |
| [OnlyVisibleCells](../../aspose.cells/pasteoptions/onlyvisiblecells/) { get; set; } | True, yalnızca görünen hücrelerin kopyalanması anlamına gelir. |
| [OperationType](../../aspose.cells/pasteoptions/operationtype/) { get; set; } | Aralık yapıştırılırken işlem türünü alır ve ayarlar. |
| [PasteType](../../aspose.cells/pasteoptions/pastetype/) { get; set; } | Yapıştırma özel türü. |
| [ShiftFormulasOfShapes](../../aspose.cells/pasteoptions/shiftformulasofshapes/) { get; set; } | Aralıklar kopyalanırken şekillerin formüllerinin kaydırılıp kaydırılmayacağını gösterir. |
| [SkipBlanks](../../aspose.cells/pasteoptions/skipblanks/) { get; set; } | Boş hücrelerin atlanıp atlanmayacağını gösterir. |
| [Transpose](../../aspose.cells/pasteoptions/transpose/) { get; set; } | Aralık yapıştırıldığında satır ve sütunların yer değiştirmesi için True. Varsayılan değer False. |

### Örnekler

```csharp
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsDemo
    {
        public static void PasteOptionsExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // İlk çalışma sayfasına bazı veriler ekleyin
            sheet.Cells["A1"].PutValue("Hello");
            sheet.Cells["A2"].PutValue("World");
            sheet.Cells["A3"].PutValue(123);

            // Başka bir çalışma sayfası oluşturun
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");

            // Kaynak aralığı tanımla
            Aspose.Cells.Range sourceRange = sheet.Cells.CreateRange("A1:A3");

            // Hedef aralığı tanımla
            Aspose.Cells.Range destRange = sheet2.Cells.CreateRange("B1:B3");

            // PasteOptions nesnesi oluşturun
            PasteOptions pasteOptions = new PasteOptions
            {
                PasteType = PasteType.Values,
                SkipBlanks = true,
                OnlyVisibleCells = false,
                Transpose = false,
                OperationType = PasteOperationType.None,
                IgnoreLinksToOriginalFile = true
            };

            // Belirtilen yapıştırma seçenekleriyle aralığı kopyalayın
            destRange.Copy(sourceRange, pasteOptions);

            // Çalışma kitabını kaydedin
            workbook.Save("PasteOptionsExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


