---
title: "Sınıf Cell"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Cell sınıfı. Tek bir Çalışma kitabı hücresini temsil eden nesneyi kapsüller."
type: docs
url: /tr/net/aspose.cells/cell/
---
## Cell class

Tek bir Workbook hücresini temsil eden nesneyi kapsüller.

```csharp
public class Cell
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [BoolValue](../../aspose.cells/cell/boolvalue/) { get; } | Hücrede bulunan boolean değeri alır. |
| [Column](../../aspose.cells/cell/column/) { get; } | Hücrenin sütun numarasını (sıfır tabanlı) alır. |
| [Comment](../../aspose.cells/cell/comment/) { get; } | Bu hücrenin yorumunu alır. |
| [ContainsExternalLink](../../aspose.cells/cell/containsexternallink/) { get; } | Bu hücrenin harici bir bağlantı içerip içermediğini gösterir. Yalnızca hücre bir formül hücresi olduğunda geçerlidir. |
| [DateTimeValue](../../aspose.cells/cell/datetimevalue/) { get; } | Hücrede bulunan DateTime değerini alır. |
| [DisplayStringValue](../../aspose.cells/cell/displaystringvalue/) { get; } | Bu hücrenin, hücrenin görüntüleme stiline göre biçimlendirilmiş dize değerini alır. |
| [DoubleValue](../../aspose.cells/cell/doublevalue/) { get; } | Hücrede bulunan double değerini alır. |
| [EmbeddedImage](../../aspose.cells/cell/embeddedimage/) { get; set; } | Hücredeki gömülü resmi alır ve ayarlar. |
| [FloatValue](../../aspose.cells/cell/floatvalue/) { get; } | Hücrede bulunan float değerini alır. |
| [Formula](../../aspose.cells/cell/formula/) { get; set; } | `Cell`'in bir formülünü alır veya ayarlar. |
| [FormulaLocal](../../aspose.cells/cell/formulalocal/) { get; set; } | Hücrenin yerel biçimlendirilmiş formülünü al. |
| [HasCustomFunction](../../aspose.cells/cell/hascustomfunction/) { get; } | Bu hücrenin formülünde özel bir işlev (desteklenmeyen işlev) olup olmadığını denetler. |
| [HasCustomStyle](../../aspose.cells/cell/hascustomstyle/) { get; } | Bu hücrenin, ilgili satır, sütun veya çalışma kitabından devralınan varsayılan stilden farklı özel stil ayarlarına sahip olup olmadığını gösterir. |
| [HtmlString](../../aspose.cells/cell/htmlstring/) { get; set; } | Bu hücrede veri ve bazı biçimleri içeren html dizesini alır ve ayarlar. |
| [IntValue](../../aspose.cells/cell/intvalue/) { get; } | Hücrede bulunan tam sayı değerini alır. |
| [IsArrayFormula](../../aspose.cells/cell/isarrayformula/) { get; } | Hücre formülünün bir dizi formülü olup olmadığını gösterir. |
| [IsArrayHeader](../../aspose.cells/cell/isarrayheader/) { get; } | Hücrenin formülünün bir dizi formülü olduğunu ve dizinin ilk hücresi olduğunu gösterir. |
| [IsCheckBoxStyle](../../aspose.cells/cell/ischeckboxstyle/) { get; set; } | Bu hücrenin bir onay kutusu olarak ayarlanıp ayarlanmadığını gösterir. |
| [IsDynamicArrayFormula](../../aspose.cells/cell/isdynamicarrayformula/) { get; } | Hücrenin formülünün dinamik dizi formülü (true) mı yoksa eski dizi formülü (false) mı olduğunu gösterir. |
| [IsErrorValue](../../aspose.cells/cell/iserrorvalue/) { get; } | Bu hücrenin değerinin bir hata olup olmadığını kontrol eder. |
| [IsFormula](../../aspose.cells/cell/isformula/) { get; } | Belirtilen hücrenin formül içerip içermediğini temsil eder. |
| [IsInArray](../../aspose.cells/cell/isinarray/) { get; } | (**Obsolete.**) Hücre formülünün bir dizi formülü olup olmadığını gösterir. |
| [IsInTable](../../aspose.cells/cell/isintable/) { get; } | (**Obsolete.**) Bu hücrenin tablo formülünün bir parçası olup olmadığını gösterir. |
| [IsMerged](../../aspose.cells/cell/ismerged/) { get; } | Bir hücrenin birleştirilmiş bir aralığın parçası olup olmadığını kontrol eder. |
| [IsNumericValue](../../aspose.cells/cell/isnumericvalue/) { get; } | Bu hücrenin değerinin sayısal (int, double ve datetime) olup olmadığını gösterir |
| [IsSharedFormula](../../aspose.cells/cell/issharedformula/) { get; } | Hücre formülünün paylaşılan bir formülün parçası olup olmadığını gösterir. |
| [IsStyleSet](../../aspose.cells/cell/isstyleset/) { get; } | Hücrenin stilinin ayarlanıp ayarlanmadığını gösterir. False dönerse, bu hücrenin varsayılan hücre biçimine sahip olduğu anlamına gelir. |
| [IsTableFormula](../../aspose.cells/cell/istableformula/) { get; } | Bu hücrenin tablo formülünün bir parçası olup olmadığını gösterir. |
| [Name](../../aspose.cells/cell/name/) { get; } | Hücrenin adını alır. |
| [NumberCategoryType](../../aspose.cells/cell/numbercategorytype/) { get; } | Bu hücrenin sayı biçimlendirmesinin kategori türünü temsil eder. |
| [Picture](../../aspose.cells/cell/picture/) { get; } | Bu hücrede gömülü görüntüyü temsil eden bir [`Picture`](../../aspose.cells.drawing/picture/) örneğini alır veya bu hücrede gömülü görüntü yoksa null döner. |
| [R1C1Formula](../../aspose.cells/cell/r1c1formula/) { get; set; } | `Cell`'in R1C1 formülünü alır veya ayarlar. |
| [Row](../../aspose.cells/cell/row/) { get; } | Hücrenin satır numarasını (sıfır tabanlı) alır. |
| [SharedStyleIndex](../../aspose.cells/cell/sharedstyleindex/) { get; } | Stil havuzundaki hücrenin paylaşılan stil indeksini alır. |
| [StringValue](../../aspose.cells/cell/stringvalue/) { get; } | Hücrede bulunan string değerini alır. Eğer bu hücrenin tipi string ise, doğrudan string değerini döndürür. Diğer hücre tipleri için, biçimlendirilmiş string değer (bu hücrenin belirtilen stiliyle biçimlendirilmiş) döndürülür. Biçimlendirilmiş hücre değeri, bir hücreyi metin olarak kopyaladığınızda (örneğin hücreyi metin düzenleyicisine kopyalama veya csv'ye dışa aktarma) Excel'den alabileceğiniz değerle aynıdır. |
| [StringValueWithoutFormat](../../aspose.cells/cell/stringvaluewithoutformat/) { get; } | (**Obsolete.**) Hücrenin değerini herhangi bir format olmadan string olarak alır. |
| [Type](../../aspose.cells/cell/type/) { get; } | Hücre değer tipini temsil eder. |
| [Value](../../aspose.cells/cell/value/) { get; set; } | Bu hücrede bulunan değeri alır/ayarlar. |
| [Worksheet](../../aspose.cells/cell/worksheet/) { get; } | Üst çalışma sayfasını alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Calculate](../../aspose.cells/cell/calculate/)(CalculationOptions) | Hücrenin formülünü hesaplar. |
| [Characters](../../aspose.cells/cell/characters/)(int, int) | Hücre metni içindeki bir karakter aralığını temsil eden bir Characters nesnesi döndürür. |
| [Copy](../../aspose.cells/cell/copy/)(Cell) | Bir kaynak hücreden verileri kopyalar. |
| [Equals](../../aspose.cells/cell/equals/#equals)(Cell) | Bu nesnenin aynı hücreye başka bir hücre nesnesiyle referans verip vermediğini kontrol eder. |
| override [Equals](../../aspose.cells/cell/equals/#equals_1)(object) | Bu nesnenin aynı hücreye başka bir nesneyle referans verip vermediğini kontrol eder. |
| [GetArrayRange](../../aspose.cells/cell/getarrayrange/)() | Hücrenin formülü bir dizi formülü ise dizi aralığını alır. |
| [GetCharacters](../../aspose.cells/cell/getcharacters/#getcharacters)() | Hücre metni içinde bir karakter aralığını temsil eden tüm Characters nesnelerini döndürür. |
| [GetCharacters](../../aspose.cells/cell/getcharacters/#getcharacters_1)(bool) | Hücre metni içinde bir karakter aralığını temsil eden tüm Characters nesnelerini döndürür. |
| [GetConditionalFormattingResult](../../aspose.cells/cell/getconditionalformattingresult/)() | Koşullu biçimlendirme sonucunu al. |
| [GetDependents](../../aspose.cells/cell/getdependents/)(bool) | Formülü doğrudan bu hücreye referans veren tüm hücreleri al. |
| [GetDependentsInCalculation](../../aspose.cells/cell/getdependentsincalculation/)(bool) | Hesaplanan sonucu bu hücreye bağlı olan tüm hücreleri al. |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle/#getdisplaystyle)() | Bu hücrenin görüntüleme stilini al. |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle/#getdisplaystyle_2)(bool) | Bu hücrenin görüntüleme stilini al. |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle/#getdisplaystyle_1)(BorderType) | Bu hücrenin görüntüleme stilini al. |
| [GetFormatConditions](../../aspose.cells/cell/getformatconditions/)() | Bu hücreye uygulanan biçim koşullarını al. |
| [GetFormula](../../aspose.cells/cell/getformula/)(bool, bool) | Bu hücrenin formülünü al. |
| override [GetHashCode](../../aspose.cells/cell/gethashcode/)() | Belirli bir tip için hash işlevi olarak hizmet eder. |
| [GetHeightOfValue](../../aspose.cells/cell/getheightofvalue/)() | Değerin yüksekliğini piksel biriminde al. |
| [GetHtmlString](../../aspose.cells/cell/gethtmlstring/)(bool) | Bu hücredeki veri ve bazı biçimleri içeren html dizesini al. |
| [GetLeafs](../../aspose.cells/cell/getleafs/#getleafs)() | (**Obsolete.**) Bu hücreye doğrudan referans veren ve hücre değiştirildiğinde güncellenmesi gereken tüm hücreleri al. |
| [GetLeafs](../../aspose.cells/cell/getleafs/#getleafs_1)(bool) | (**Obsolete.**) Bu hücre değiştirildiğinde güncellenecek tüm hücreleri al. |
| [GetMergedRange](../../aspose.cells/cell/getmergedrange/)() | Birleştirilmiş bir aralığı temsil eden bir [`Range`](../range/) nesnesi döndürür. |
| [GetPrecedents](../../aspose.cells/cell/getprecedents/)() | Bu hücrenin formülünde görünen tüm referansları al. |
| [GetPrecedentsInCalculation](../../aspose.cells/cell/getprecedentsincalculation/)() | Bu hücrenin formülü hesaplanırken kullandığı tüm öncülleri (geçerli çalışma kitabındaki hücre referansları) al. |
| [GetRichValue](../../aspose.cells/cell/getrichvalue/)() | Hücrenin zengin değerini al. |
| [GetStringValue](../../aspose.cells/cell/getstringvalue/)(CellValueFormatStrategy) | Belirli bir biçimlendirme stratejisiyle dize değerini al. |
| [GetStyle](../../aspose.cells/cell/getstyle/#getstyle)() | Hücre stilini al. |
| [GetStyle](../../aspose.cells/cell/getstyle/#getstyle_1)(bool) | checkBorders true ise, diğer hücrelerin kenarlıklarının bu hücrenin stilini etkileyip etkilemeyeceğini kontrol et. |
| [GetTable](../../aspose.cells/cell/gettable/)() | Bu hücreyi içeren tabloyu al. |
| [GetValidation](../../aspose.cells/cell/getvalidation/)() | Bu hücreye uygulanan doğrulamayı al. |
| [GetValidationValue](../../aspose.cells/cell/getvalidationvalue/)() | Bu hücreye uygulanan doğrulamanın değerini alır. |
| [GetWidthOfValue](../../aspose.cells/cell/getwidthofvalue/)() | Değerin piksel birimindeki genişliğini alır. |
| [InsertText](../../aspose.cells/cell/inserttext/)(int, string) | Hücreye bazı karakterler ekler. Hücre zengin biçimlendirilmişse, bu yöntem orijinal biçimlendirmeyi koruyabilir. |
| [IsRichText](../../aspose.cells/cell/isrichtext/)() | Bu hücrenin dize değerinin zengin biçimlendirilmiş bir metin olup olmadığını gösterir. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue)(bool) | Hücreye bir mantıksal değer koyar. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_3)(DateTime) | Hücreye bir DateTime değeri koyar. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_1)(double) | Hücreye bir double değeri koyar. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_2)(int) | Hücreye bir tam sayı değeri koyar. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_4)(object) | Hücreye bir nesne değeri koyar. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_5)(string) | Hücreye bir dize değeri koyar. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_6)(string, bool) | Hücreye bir dize değeri koyar ve uygun olduğunda değeri başka bir veri tipine dönüştürür. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_7)(string, bool, bool) | Hücreye bir değer koyar, uygun olduğunda değer başka bir veri tipine dönüştürülür ve hücrenin sayı biçimi sıfırlanır. |
| [RemoveArrayFormula](../../aspose.cells/cell/removearrayformula/)(bool) | Dizi formülünü kaldır. |
| [Replace](../../aspose.cells/cell/replace/)(string, string, ReplaceOptions) | Hücrenin metnini seçeneklerle değiştir. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula/#setarrayformula)(string, int, int) | Bir dizi formülünü (CTRL+SHIFT+ENTER ile MS Excel'de girilen eski dizi formülü) hücre aralığına ayarlar. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula/#setarrayformula_1)(string, int, int, FormulaParseOptions) | Bir dizi formülünü hücre aralığına ayarlar. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula/#setarrayformula_3)(string, int, int, bool, bool) | (**Obsolete.**) Bir dizi formülünü hücre aralığına ayarlar. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula/#setarrayformula_2)(string, int, int, FormulaParseOptions, object[][]) | Bir dizi formülünü hücre aralığına ayarlar. |
| [SetCharacters](../../aspose.cells/cell/setcharacters/)(FontSetting[]) | Hücrenin zengin metin biçimini ayarlar. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula/#setdynamicarrayformula)(string, FormulaParseOptions, bool) | Dinamik dizi formülünü ayarlar ve mümkünse formülün komşu hücrelere yayılmasını sağlar. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula/#setdynamicarrayformula_1)(string, FormulaParseOptions, object[][], bool, bool) | Dinamik dizi formülünü ayarlar ve mümkünse formülün komşu hücrelere yayılmasını sağlar. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula/#setdynamicarrayformula_2)(string, FormulaParseOptions, object[][], bool, bool, CalculationOptions) | Dinamik dizi formülünü ayarlar ve mümkünse formülün komşu hücrelere yayılmasını sağlar. |
| [SetFormula](../../aspose.cells/cell/setformula/#setformula)(string, FormulaParseOptions) | Formülü ve formülün değerini (hesaplanan sonuç) ayarlar. |
| [SetFormula](../../aspose.cells/cell/setformula/#setformula_3)(string, object) | Formülü ve formülün değerini (hesaplanan sonuç) ayarlar. |
| [SetFormula](../../aspose.cells/cell/setformula/#setformula_1)(string, FormulaParseOptions, object) | Formülü ve formülün değerini (hesaplanan sonuç) ayarlar. |
| [SetFormula](../../aspose.cells/cell/setformula/#setformula_2)(string, bool, bool, object) | (**Obsolete.**) Formülü ve formülün değerini ayarlar. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula/#setsharedformula)(string, int, int) | Paylaşılan formülleri hücre aralığına ayarlar. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula/#setsharedformula_1)(string, int, int, FormulaParseOptions) | Paylaşılan formülleri hücre aralığına ayarlar. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula/#setsharedformula_3)(string, int, int, bool, bool) | (**Obsolete.**) Bir formülü hücre aralığına ayarlar. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula/#setsharedformula_2)(string, int, int, FormulaParseOptions, object[][]) | Paylaşılan formülleri hücre aralığına ayarlar. |
| [SetStyle](../../aspose.cells/cell/setstyle/#setstyle)(Style) | Hücre stilini ayarlar. |
| [SetStyle](../../aspose.cells/cell/setstyle/#setstyle_2)(Style, bool) | Stilin değiştirilmiş özelliğini hücreye uygular. |
| [SetStyle](../../aspose.cells/cell/setstyle/#setstyle_1)(Style, StyleFlag) | Bayraklara göre hücre stilini uygula. |
| [SetTableFormula](../../aspose.cells/cell/settableformula/#settableformula_2)(int, int, string, bool, object[][]) | Bu hücreden başlayarak verilen aralık için tek değişkenli veri tablosu oluştur. |
| [SetTableFormula](../../aspose.cells/cell/settableformula/#settableformula_3)(int, int, string, string, object[][]) | Bu hücreden başlayarak verilen aralık için iki değişkenli veri tablosu oluştur. |
| [SetTableFormula](../../aspose.cells/cell/settableformula/#settableformula)(int, int, int, int, bool, object[][]) | Bu hücreden başlayarak verilen aralık için tek değişkenli veri tablosu oluştur. |
| [SetTableFormula](../../aspose.cells/cell/settableformula/#settableformula_1)(int, int, int, int, int, int, object[][]) | Bu hücreden başlayarak verilen aralık için iki değişkenli veri tablosu oluştur. |
| [ToJson](../../aspose.cells/cell/tojson/)() | `Cell` nesnesini JSON yapı verisine dönüştür. |
| override [ToString](../../aspose.cells/cell/tostring/)() | Geçerli Cell nesnesini temsil eden bir dize döndürür. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellDemo
    {
        public static void CellExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            // Hücreler koleksiyonuna eriş
            Cells cells = worksheet.Cells;

            // Bir dizeyi hücreye yerleştir
            Cell cell = cells[0, 0];
            cell.PutValue("Hello");

            // Bir tam sayıyı hücreye yerleştir
            cell = cells["B1"];
            cell.PutValue(12);

            // Bir double değeri hücreye yerleştir
            cell = cells[0, 2];
            cell.PutValue(-1.234);

            // Bir formülü hücreye yerleştir
            cell = cells["D1"];
            cell.Formula = "=B1 + C1";

            // Bir birleşik formül: "sum(average(b1,c1), b1)" i b2 hücresine yerleştir
            cell = cells["B2"];
            cell.Formula = "=sum(average(b1,c1), b1)";

            // Bir hücrenin stilini ayarla
            Style style = cell.GetStyle();
            // Arka plan rengini ayarla
            style.BackgroundColor = System.Drawing.Color.Yellow;
            // Bir hücrenin yazı tipini ayarla
            style.Font.Name = "Courier New";
            style.VerticalAlignment = TextAlignmentType.Top;
            cell.SetStyle(style);

            // Çalışma kitabını kaydedin
            workbook.Save("CellExample.xlsx");
            workbook.Save("CellExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


