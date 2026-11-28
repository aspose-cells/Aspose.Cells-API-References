---
title: "Sınıf CopyOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.CopyOptions sınıfı. Kopyalama seçeneklerini temsil eder"
type: docs
url: /tr/net/aspose.cells/copyoptions/
---
## CopyOptions class

Kopyalama seçeneklerini temsil eder.

```csharp
public class CopyOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [CopyOptions](copyoptions/)() | CopyOptions yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ColumnCharacterWidth](../../aspose.cells/copyoptions/columncharacterwidth/) { get; set; } | Sütun genişliğinin karakter biriminde kopyalanıp kopyalanmayacağını gösterir. |
| [CopyInvalidFormulasAsValues](../../aspose.cells/copyoptions/copyinvalidformulasasvalues/) { get; set; } | Formül hedef konum için geçerli değilse, yalnızca değerleri kopyalar. |
| [CopyNames](../../aspose.cells/copyoptions/copynames/) { get; set; } | İsimlerin kopyalanıp kopyalanmayacağını gösterir. |
| [ExtendToAdjacentRange](../../aspose.cells/copyoptions/extendtoadjacentrange/) { get; set; } | Aralığı bitişik aralığa kopyalarken aralıkların genişletilip genişletilmeyeceğini gösterir. |
| [KeepMacros](../../aspose.cells/copyoptions/keepmacros/) { get; set; } | Makroların korunup korunmayacağını gösterir; |
| [ReferToDestinationSheet](../../aspose.cells/copyoptions/refertodestinationsheet/) { get; set; } | Aynı dosyada aralık kopyalanırken ve grafik kaynak sayfaya referans veriyorsa, False kopyalanan grafiğin veri kaynağının değişmeyeceği anlamına gelir. True ise kopyalanan grafiğin veri kaynağının hedef sayfaya referans vereceği anlamına gelir. |
| [ReferToSheetWithSameName](../../aspose.cells/copyoptions/refertosheetwithsamename/) { get; set; } | MS Excel'de, bir çalışma sayfasını başka birine kopyalarken diğer çalışma sayfalarına referans veren formüller kopyalandığında, kopyalanan formüllerin kaynak çalışma kitabına referans vermesi gerekir. Ancak bazı durumlarda kullanıcı, kopyalanan formüllerin aynı çalışma kitabındaki aynı ada sahip çalışma sayfalarına referans vermesini isteyebilir; örneğin bu çalışma sayfaları bu kopyalama işleminden önce zaten kopyalanmışsa, bu özellik true olarak tutulmalıdır. |
| [UpdateInvalidReferencesToTargetSheet](../../aspose.cells/copyoptions/updateinvalidreferencestotargetsheet/) { get; set; } | Referans verilen çalışma sayfası kopyalanmamışsa hedef çalışma sayfasına referans verilip verilmeyeceğini gösterir. |

### Örnekler

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class CopyOptionsDemo
    {
        public static void CopyOptionsExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı veriler ekle
            sheet.Cells["A1"].PutValue("Hello");
            sheet.Cells["A2"].PutValue("World");

            // Verileri kopyalamak için yeni bir çalışma kitabı oluştur
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];

            // Bir CopyOptions nesnesi oluştur
            CopyOptions copyOptions = new CopyOptions
            {
                KeepMacros = true,
                ExtendToAdjacentRange = true,
                CopyNames = true,
                CopyInvalidFormulasAsValues = true,
                ColumnCharacterWidth = true,
                ReferToSheetWithSameName = true,
                ReferToDestinationSheet = true
            };

            // Verileri kaynak çalışma sayfasından hedef çalışma sayfasına kopyala
            destSheet.Cells.CopyRows(sheet.Cells, 0, 0, 2, copyOptions);

            // Hedef çalışma kitabını kaydet
            destWorkbook.Save("CopyOptionsExample.xlsx");
            destWorkbook.Save("CopyOptionsExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


