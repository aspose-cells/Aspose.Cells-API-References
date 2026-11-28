---
title: "Enum AutoFitMergedCellsType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.AutoFitMergedCellsType enum. Birleştirilmiş hücrelerin otomatik sığdırılma türünü temsil eder"
type: docs
url: /tr/net/aspose.cells/autofitmergedcellstype/
---
## AutoFitMergedCellsType enumeration

Birleştirilmiş hücrelerin otomatik sığdırma türünü temsil eder.

```csharp
public enum AutoFitMergedCellsType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Birleştirilmiş hücreleri yoksay. |
| FirstLine | `1` | Yalnızca ilk satırın yüksekliğini genişletir. |
| LastLine | `2` | Yalnızca son satırın yüksekliğini genişletir. |
| EachLine | `3` | Her satırın yüksekliğini genişletir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;

    public class AutoFitMergedCellsTypeDemo
    {
        public static void AutoFitMergedCellsTypeExample()
        {
            //Bir Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();
            //Yeni eklenen çalışma sayfasının referansını elde etme
            Worksheet sheet1 = workbook.Worksheets[0];

            // A1:B2 aralığını oluştur
            Range range = sheet1.Cells.CreateRange(0, 0, 2, 2);

            // Hücreleri birleştir
            range.Merge();

            // Birleştirilmiş hücre A1'e değer ekle
            sheet1.Cells[0, 0].Value = "This is test text for autofit merged cells type demo This is test text for autofit merged cells type demo";

            // Bir stil nesnesi oluşturun
            Style style = sheet1.Cells[0, 0].GetStyle();

            // Metin kaydırmayı etkinleştir
            style.IsTextWrapped = true;

            // Stili hücreye uygulayın
            sheet1.Cells[0, 0].SetStyle(style);

            // AutoFitterOptions için bir nesne oluştur
            AutoFitterOptions options = new AutoFitterOptions();

            // Yalnızca ilk satırın yüksekliğini genişletir.
            options.AutoFitMergedCellsType = AutoFitMergedCellsType.FirstLine;

            // Sayfadaki satırları (birleştirilmiş hücreler dahil) otomatik sığdır
            sheet1.AutoFitRows(options);


            int index = workbook.Worksheets.Add();
            Worksheet sheet2 = workbook.Worksheets[index];
            sheet2.Name = "Sheet2";
            // A1:B2 aralığını oluştur
            Range range2 = sheet2.Cells.CreateRange(0, 0, 2, 2);

            // Hücreleri birleştir
            range2.Merge();

            // Birleştirilmiş hücre A1'e değer ekle
            sheet2.Cells[0, 0].Value = "This is test text for autofit merged cells type demo This is test text for autofit merged cells type demo";

            // Bir stil nesnesi oluşturun
            Style style2 = sheet2.Cells[0, 0].GetStyle();

            // Metin kaydırmayı etkinleştir
            style2.IsTextWrapped = true;

            // Stili hücreye uygulayın
            sheet2.Cells[0, 0].SetStyle(style);

            // AutoFitterOptions için bir nesne oluştur
            AutoFitterOptions options2 = new AutoFitterOptions();

            // Yalnızca son satırın yüksekliğini genişletir.
            options2.AutoFitMergedCellsType = AutoFitMergedCellsType.LastLine;

            // Sayfadaki satırları (birleştirilmiş hücreler dahil) otomatik sığdır
            sheet2.AutoFitRows(options2);


            index = workbook.Worksheets.Add();
            Worksheet sheet3 = workbook.Worksheets[index];
            sheet3.Name = "Sheet3";
            // A1:B2 aralığını oluştur
            Range range3 = sheet3.Cells.CreateRange(0, 0, 2, 2);

            // Hücreleri birleştir
            range3.Merge();

            // Birleştirilmiş hücre A1'e değer ekle
            sheet3.Cells[0, 0].Value = "This is test text for autofit merged cells type demo This is test text for autofit merged cells type demo";

            // Bir stil nesnesi oluşturun
            Style style3 = sheet3.Cells[0, 0].GetStyle();

            // Metin kaydırmayı etkinleştir
            style3.IsTextWrapped = true;

            // Stili hücreye uygulayın
            sheet3.Cells[0, 0].SetStyle(style);

            // AutoFitterOptions için bir nesne oluştur
            AutoFitterOptions options3 = new AutoFitterOptions();

            // Her satırın yüksekliğini yalnızca genişletir.
            options3.AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine;

            // Sayfadaki satırları (birleştirilmiş hücreler dahil) otomatik sığdır
            sheet3.AutoFitRows(options3);


            index = workbook.Worksheets.Add();
            Worksheet sheet4 = workbook.Worksheets[index];
            sheet4.Name = "Sheet4";
            // A1:B2 aralığını oluştur
            Range range4 = sheet4.Cells.CreateRange(0, 0, 2, 2);

            // Hücreleri birleştir
            range4.Merge();

            // Birleştirilmiş hücre A1'e değer ekle
            sheet4.Cells[0, 0].Value = "This is test text for autofit merged cells type demo This is test text for autofit merged cells type demo";

            // Bir stil nesnesi oluşturun
            Style style4 = sheet4.Cells[0, 0].GetStyle();

            // Metin kaydırmayı etkinleştir
            style4.IsTextWrapped = true;

            // Stili hücreye uygulayın
            sheet4.Cells[0, 0].SetStyle(style);

            // AutoFitterOptions için bir nesne oluştur
            AutoFitterOptions options4 = new AutoFitterOptions();

            // Birleştirilmiş hücreleri yoksay.
            options4.AutoFitMergedCellsType = AutoFitMergedCellsType.None;

            // Sayfadaki satırları (birleştirilmiş hücreler hariç) otomatik sığdır
            sheet4.AutoFitRows(options4);

            // Çalışma kitabını kaydedin
            workbook.Save("AutoFitMergedCellsTypeExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


