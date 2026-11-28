---
title: "CellsHelper sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.CellsHelper sınıfı. Yardımcı işlevler sağlar."
type: docs
url: /tr/net/aspose.cells/cellshelper/
---
## CellsHelper class

Yardımcı işlevler sağlar.

```csharp
public class CellsHelper
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| static [AltStartPath](../../aspose.cells/cellshelper/altstartpath/) { get; set; } | Bazı dış formül referansları tarafından kullanılan alternatif başlangıç yolunu alır veya ayarlar. |
| static [CustomImplementationFactory](../../aspose.cells/cellshelper/customimplementationfactory/) { get; set; } | Özel uygulama ile örnekler oluşturmak için fabrikayı alır veya ayarlar. |
| static [DPI](../../aspose.cells/cellshelper/dpi/) { get; set; } | Makinenin DPI değerini alır. |
| static [IsCloudPlatform](../../aspose.cells/cellshelper/iscloudplatform/) { get; set; } | Bulut platformunda (Azure, AWSLambda vb.) çalışırken lütfen bu özelliği True olarak ayarlayın, |
| static [LibraryPath](../../aspose.cells/cellshelper/librarypath/) { get; set; } | Bazı dış formül referansları tarafından kullanılan kütüphane yolunu alır veya ayarlar. |
| static [SignificantDigits](../../aspose.cells/cellshelper/significantdigits/) { get; set; } | (**Obsolete.**) Önemli basamak sayısını alır ve ayarlar. Varsayılan değer 17'dir. |
| static [SignificantDigitsType](../../aspose.cells/cellshelper/significantdigitstype/) { get; set; } | Sayısal değerleri çıkartmak için varsayılan önemli basamak tipini alır ve ayarlar. Varsayılan değer G17'dir. |
| static [StartupPath](../../aspose.cells/cellshelper/startuppath/) { get; set; } | Bazı dış formül referansları tarafından kullanılan başlangıç yolunu alır veya ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| static [AddAddInFunction](../../aspose.cells/cellshelper/addaddinfunction/)(string, int, int, ParameterType[], ParameterType) | (**Obsolete.**) Eklenti işlevi ekle. |
| static [CellIndexToName](../../aspose.cells/cellshelper/cellindextoname/)(int, int) | Satır ve sütun indekslerine göre hücre adını alır. |
| static [CellNameToIndex](../../aspose.cells/cellshelper/cellnametoindex/)(string, out int, out int) | Hücre adını temel alarak hücrenin satır ve sütun indekslerini alır. |
| static [ColumnIndexToName](../../aspose.cells/cellshelper/columnindextoname/)(int) | Sütun indeksine göre sütun adını alır. |
| static [ColumnNameToIndex](../../aspose.cells/cellshelper/columnnametoindex/)(string) | Sütun adına göre sütun indeksini alır. |
| static [ConvertA1FormulaToR1C1](../../aspose.cells/cellshelper/converta1formulator1c1/)(string, int, int) | (**Obsolete.**) Hücrenin A1 formülünü r1c1 formülüne dönüştürür. |
| static [ConvertR1C1FormulaToA1](../../aspose.cells/cellshelper/convertr1c1formulatoa1/)(string, int, int) | (**Obsolete.**) Hücrenin r1c1 formülünü A1 formülüne dönüştürür. |
| static [CreateSafeSheetName](../../aspose.cells/cellshelper/createsafesheetname/#createsafesheetname)(string) | Verilen sayfa adını kontrol eder ve gerektiğinde geçerli bir ad oluşturur. Verilen sayfa adı Excel sayfa adı kurallarına uygunsa, onu döndürür. Aksi takdirde, uzunluğu limiti aşarsa dize kesilir ve geçersiz karakterler ' ' ile değiştirilir, ardından yeniden oluşturulmuş dize değeri döndürülür. |
| static [CreateSafeSheetName](../../aspose.cells/cellshelper/createsafesheetname/#createsafesheetname_1)(string, char) | Verilen sayfa adını kontrol eder ve gerektiğinde geçerli bir ad oluşturur. Verilen sayfa adı Excel sayfa adı kurallarına uygunsa, onu döndürür. Aksi takdirde, uzunluğu limiti aşarsa dize kesilir ve geçersiz karakterler verilen karakterle değiştirilir, ardından yeniden oluşturulmuş dize değeri döndürülür. |
| static [GetCacheFolder](../../aspose.cells/cellshelper/getcachefolder/)() | Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasörü alır. |
| static [GetDateTimeFromDouble](../../aspose.cells/cellshelper/getdatetimefromdouble/)(double, bool) | Double değerini tarih saat değerine dönüştür. |
| static [GetDoubleFromDateTime](../../aspose.cells/cellshelper/getdoublefromdatetime/)(DateTime, bool) | Tarih saat değerini double değere dönüştür. |
| static [GetTextWidth](../../aspose.cells/cellshelper/gettextwidth/)(string, Font, double) | Metnin genişliğini nokta biriminde al. |
| static [GetUsedColors](../../aspose.cells/cellshelper/getusedcolors/)(Workbook) | Çalışma kitabında kullanılan tüm renkleri alır. |
| static [GetVersion](../../aspose.cells/cellshelper/getversion/)() | Sürüm numarasını al. |
| static [MergeFiles](../../aspose.cells/cellshelper/mergefiles/)(string[], string, string) | Bazı büyük xls dosyalarını tek bir xls dosyasına birleştirir. |
| static [NeedQuoteInFormula](../../aspose.cells/cellshelper/needquoteinformula/)(string) | Sayfa adının tek tırnak içinde olup olmayacağını gösterir. |
| static [RowIndexToName](../../aspose.cells/cellshelper/rowindextoname/)(int) | Satır indeksine göre satır adını alır. |
| static [RowNameToIndex](../../aspose.cells/cellshelper/rownametoindex/)(string) | Satır adına göre satır indeksini alır. |
| static [SetCacheFolder](../../aspose.cells/cellshelper/setcachefolder/)(string) | Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasörü ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperDemo
    {
        public static void CellsHelperExample()
        {
            // CellsHelper özelliklerini ayarlama
            CellsHelper.SignificantDigits = 15;
            CellsHelper.DPI = 96.0;
            CellsHelper.StartupPath = "C:\\Program Files\\Aspose\\Cells";
            CellsHelper.AltStartPath = "D:\\Aspose\\Cells";
            CellsHelper.LibraryPath = "E:\\Aspose\\Cells\\Library";
            CellsHelper.IsCloudPlatform = true;

            // CustomImplementationFactory'nin başka bir yerde zaten tanımlandığı ve örneklenmiş olduğu varsayılıyor
            CellsHelper.CustomImplementationFactory = new CustomImplementationFactory();

            // CellsHelper özelliklerinin kullanımını gösterme
            Console.WriteLine("Significant Digits: " + CellsHelper.SignificantDigits);
            Console.WriteLine("DPI: " + CellsHelper.DPI);
            Console.WriteLine("Startup Path: " + CellsHelper.StartupPath);
            Console.WriteLine("Alternate Startup Path: " + CellsHelper.AltStartPath);
            Console.WriteLine("Library Path: " + CellsHelper.LibraryPath);
            Console.WriteLine("Is Cloud Platform: " + CellsHelper.IsCloudPlatform);

            // CustomImplementationFactory kullanım örneği
            var memoryStream = CellsHelper.CustomImplementationFactory.CreateMemoryStream();
            Console.WriteLine("MemoryStream created with CustomImplementationFactory: " + (memoryStream != null));

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


