---
title: "Sınıf SheetSet"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Rendering.SheetSet sınıfı. Bir dizi sayfayı tanımlar"
type: docs
url: /tr/net/aspose.cells.rendering/sheetset/
---
## SheetSet class

Bir dizi çalışma sayfasını tanımlar.

```csharp
public class SheetSet
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [SheetSet](sheetset/#constructor)(params int[]) | Tam sayfa indekslerine göre bir sayfa seti oluşturur. |
| [SheetSet](sheetset/#constructor_1)(params string[]) | Tam sayfa adlarına göre bir sayfa seti oluşturur. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| static [Active](../../aspose.cells.rendering/sheetset/active/) { get; } | Çalışma kitabının aktif sayfasını içeren bir set alır. |
| static [All](../../aspose.cells.rendering/sheetset/all/) { get; } | Çalışma kitabının tüm sayfalarını orijinal sıralarında içeren bir set alır. |
| static [Visible](../../aspose.cells.rendering/sheetset/visible/) { get; } | Çalışma kitabının görünür sayfalarını orijinal sıralarında içeren bir set alır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetSetDemo
    {
        public static void SheetSetExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı veriler ekle
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(456);   

            worksheet = workbook.Worksheets.Add("test1");
            worksheet.Cells["A1"].PutValue("test Data");
            worksheet.Cells["A2"].PutValue(234);
            worksheet.Cells["A3"].PutValue(333);
            worksheet.IsVisible = false;

            worksheet = workbook.Worksheets.Add("test2");
            worksheet.Cells["A1"].PutValue("test Data222");
            worksheet.Cells["A2"].PutValue(234444);
            worksheet.Cells["A3"].PutValue(333555);

            workbook.Worksheets.ActiveSheetIndex = 0;

            // PdfSaveOptions nesnesi oluşturun
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // SheetSet özelliğini yalnızca aktif sayfayı içerecek şekilde ayarlayın
            pdfSaveOptions.SheetSet = SheetSet.Active;

            // Çalışma kitabını bir PDF dosyasına kaydedin
            workbook.Save("SheetSetExample_ActiveSheet.pdf", pdfSaveOptions);

            // SheetSet özelliğini tüm görünür sayfaları içerecek şekilde ayarlayın
            pdfSaveOptions.SheetSet = SheetSet.Visible;

            // Çalışma kitabını bir PDF dosyasına kaydedin
            workbook.Save("SheetSetExample_VisibleSheets.pdf", pdfSaveOptions);

            // SheetSet özelliğini tüm sayfaları içerecek şekilde ayarlayın
            pdfSaveOptions.SheetSet = SheetSet.All;

            // Çalışma kitabını bir PDF dosyasına kaydedin
            workbook.Save("SheetSetExample_AllSheets.pdf", pdfSaveOptions);

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


