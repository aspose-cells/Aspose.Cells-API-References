---
title: "GlobalizationSettings sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GlobalizationSettings sınıfı. Küreselleştirme ayarlarını temsil eder"
type: docs
url: /tr/net/aspose.cells/globalizationsettings/
---
## GlobalizationSettings class

Küreselleştirme ayarlarını temsil eder.

```csharp
public class GlobalizationSettings
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [GlobalizationSettings](globalizationsettings/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ChartSettings](../../aspose.cells/globalizationsettings/chartsettings/) { get; set; } | Grafik için küreselleştirme ayarlarını alır veya ayarlar. |
| virtual [ColumnSeparatorOfFormulaArray](../../aspose.cells/globalizationsettings/columnseparatorofformulaarray/) { get; } | Formülde dizi satır verilerindeki öğeler için ayırıcıyı alır. |
| virtual [ListSeparator](../../aspose.cells/globalizationsettings/listseparator/) { get; } | Liste, fonksiyon parametreleri, ... vb. için ayırıcıyı alır. |
| [PivotSettings](../../aspose.cells/globalizationsettings/pivotsettings/) { get; set; } | Özet tablo için küreselleştirme ayarlarını alır veya ayarlar. |
| virtual [RowSeparatorOfFormulaArray](../../aspose.cells/globalizationsettings/rowseparatorofformulaarray/) { get; } | Formülde dizi verilerindeki satırlar için ayırıcıyı alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| virtual [Compare](../../aspose.cells/globalizationsettings/compare/)(string, string, bool) | İki dize değerini belirli karşılaştırma kurallarına göre karşılaştırır. |
| virtual [GetAllName](../../aspose.cells/globalizationsettings/getallname/)() | (**Obsolete.**) PivotTable'daki "(All)" etiketinin adını alır. |
| virtual [GetBooleanValueString](../../aspose.cells/globalizationsettings/getbooleanvaluestring/)(bool) | Hücrenin boolean değerinin görüntüleme dizesi değerini alır |
| virtual [GetCollationKey](../../aspose.cells/globalizationsettings/getcollationkey/)(string, bool) | Dizeyi belirli karşılaştırma kurallarına göre karşılaştırılabilir bir nesneye dönüştürür. |
| virtual [GetColumnLabelsOfPivotTable](../../aspose.cells/globalizationsettings/getcolumnlabelsofpivottable/)() | (**Obsolete.**) PivotTable'daki "Column Labels" etiketinin adını alır. |
| virtual [GetCommentTitleName](../../aspose.cells/globalizationsettings/getcommenttitlename/)(CommentTitleType) | Yorum başlığı türüne göre yerel ayara bağlı yorum başlığı adını alır. |
| virtual [GetDataFieldHeaderNameOfPivotTable](../../aspose.cells/globalizationsettings/getdatafieldheadernameofpivottable/)() | (**Eski.**) PivotTable'taki değer alanı başlığı adını alır. |
| virtual [GetDefaultSheetName](../../aspose.cells/globalizationsettings/getdefaultsheetname/)() | Çalışma sayfası otomatik olarak eklenirken varsayılan sayfa adını alır. Varsayılan "Sheet". |
| virtual [GetEmptyDataName](../../aspose.cells/globalizationsettings/getemptydataname/)() | (**Eski.**) PivotTable'taki "(blank)" etiketi adını alır. |
| virtual [GetErrorValueString](../../aspose.cells/globalizationsettings/geterrorvaluestring/)(string) | Hücrenin hata değerinin görüntüleme dizesi değerini alır |
| virtual [GetGrandTotalName](../../aspose.cells/globalizationsettings/getgrandtotalname/)(ConsolidationFunction) | Fonksiyonun genel toplam adını alır. |
| virtual [GetLocalBuiltInName](../../aspose.cells/globalizationsettings/getlocalbuiltinname/)(string) | Verilen standart metne göre yerel ayara bağlı yerleşik Name metnini alır. |
| virtual [GetLocalFunctionName](../../aspose.cells/globalizationsettings/getlocalfunctionname/)(string) | Verilen standart fonksiyon adına göre yerel ayara bağlı fonksiyon adını alır. |
| virtual [GetMultipleItemsName](../../aspose.cells/globalizationsettings/getmultipleitemsname/)() | (**Eski.**) PivotTable'taki "(Multiple Items)" etiketi adını alır. |
| virtual [GetPivotGrandTotalName](../../aspose.cells/globalizationsettings/getpivotgrandtotalname/)() | (**Eski.**) PivotTable'taki "Grand Total" etiketi adını alır. |
| virtual [GetPivotTotalName](../../aspose.cells/globalizationsettings/getpivottotalname/)() | (**Eski.**) PivotTable'taki "Total" etiketi adını alır. PivotTable veri alanında iki veya daha fazla PivotField içerdiğinde bu yöntemi geçersiz kılmanız gerekir. |
| virtual [GetProtectionNameOfPivotTable](../../aspose.cells/globalizationsettings/getprotectionnameofpivottable/)() | (**Eski.**) PivotTable'taki koruma adını alır. |
| virtual [GetRowLabelsNameOfPivotTable](../../aspose.cells/globalizationsettings/getrowlabelsnameofpivottable/)() | (**Eski.**) PivotTable'taki "Row Labels" etiketi adını alır. |
| virtual [GetStandardBuiltInName](../../aspose.cells/globalizationsettings/getstandardbuiltinname/)(string) | Verilen yerel ayara bağlı metne göre yerleşik Name'in standart metnini alır. |
| virtual [GetStandardFunctionName](../../aspose.cells/globalizationsettings/getstandardfunctionname/)(string) | Verilen yerel ayara bağlı fonksiyon adına göre standart fonksiyon adını alır. |
| virtual [GetStandardHeaderFooterFontStyleName](../../aspose.cells/globalizationsettings/getstandardheaderfooterfontstylename/)(string) | Verilen yerel font stiline göre Başlık/Altbilgi için standart İngilizce yazı tipi stil adını (Regular, Bold, Italic) alır. |
| virtual [GetSubTotalName](../../aspose.cells/globalizationsettings/getsubtotalname/)(PivotFieldSubtotalType) | (**Eski.**) PivotTable'taki [`PivotFieldSubtotalType`](../../aspose.cells.pivot/pivotfieldsubtotaltype/) tipinin adını alır. |
| virtual [GetTableRowTypeOfAll](../../aspose.cells/globalizationsettings/gettablerowtypeofall/)() | Referans alınan tablodaki tüm satırları içeren tablo satırlarının tip adını alır. Varsayılan "All" olduğundan, "#All" formülünde referans alınan tablonun tüm satırlarını temsil eder. |
| virtual [GetTableRowTypeOfCurrent](../../aspose.cells/globalizationsettings/gettablerowtypeofcurrent/)() | Referans alınan tablodaki mevcut satırı içeren tablo satırlarının tip adını alır. Varsayılan "This Row" olduğundan, "#This Row" formülünde referans alınan tablonun mevcut satırını temsil eder. |
| virtual [GetTableRowTypeOfData](../../aspose.cells/globalizationsettings/gettablerowtypeofdata/)() | Referans verilen tablonun veri bölgesini içeren tablo satırlarının tip adını alır. Varsayılan "Data"dır, bu yüzden formülde "#Data" tabloyun veri bölgesini temsil eder. |
| virtual [GetTableRowTypeOfHeaders](../../aspose.cells/globalizationsettings/gettablerowtypeofheaders/)() | Tablo başlığını içeren tablo satırlarının tip adını alır. Varsayılan "Headers"dır, bu yüzden formülde "#Headers" tablo başlığını temsil eder. |
| virtual [GetTableRowTypeOfTotals](../../aspose.cells/globalizationsettings/gettablerowtypeoftotals/)() | Referans alınan tablonun toplam satırını içeren tablo satırlarının tip adını alır. Varsayılan "Totals" olduğundan, "#Totals" formülünde referans alınan tablonun toplam satırını temsil eder. |
| virtual [GetTotalName](../../aspose.cells/globalizationsettings/gettotalname/)(ConsolidationFunction) | Fonksiyonun toplam adını alır. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassGlobalizationSettingsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Örnek veri ekleyin.
            cells["A1"].PutValue("Region");
            cells["B1"].PutValue("Sales");
            cells["A2"].PutValue("North");
            cells["B2"].PutValue(1000);
            cells["A3"].PutValue("South");
            cells["B3"].PutValue(2000);
            cells["A4"].PutValue("East");
            cells["B4"].PutValue(3000);
            cells["A5"].PutValue("West");
            cells["B5"].PutValue(4000);

            // Küreselleştirme ayarlarını oluştur ve uygula
            GlobalizationSettings settings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = settings;

            // Özel küreselleştirme ile alt toplam uygula
            CellArea area = CellArea.CreateCellArea(0, 0, 5, 1);
            cells.Subtotal(area, 0, ConsolidationFunction.Sum, new int[] { 0 }, true, false, true);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetTotalName(ConsolidationFunction functionType)
        {
            // Fonksiyon tipine göre toplam adını özelleştir
            switch (functionType)
            {
                case ConsolidationFunction.Sum:
                    return "Custom Sum";
                case ConsolidationFunction.Count:
                    return "Custom Count";
                default:
                    return base.GetTotalName(functionType);
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


