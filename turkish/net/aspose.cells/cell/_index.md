---
title: Cell
second_title: Aspose.Cells for .NET API Referansı
description: Tek bir Çalışma Kitabı hücresini temsil eden nesneyi kapsüller.
type: docs
weight: 230
url: /tr/net/aspose.cells/cell/
---
## Cell class

Tek bir Çalışma Kitabı hücresini temsil eden nesneyi kapsüller.

```csharp
public class Cell
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [BoolValue](../../aspose.cells/cell/boolvalue) { get; } | Hücrede bulunan boole değerini alır. |
| [Column](../../aspose.cells/cell/column) { get; } | Hücrenin sütun numarasını (sıfır tabanlı) alır. |
| [Comment](../../aspose.cells/cell/comment) { get; } | Bu hücrenin yorumunu alır. |
| [ContainsExternalLink](../../aspose.cells/cell/containsexternallink) { get; } | Bu hücrenin harici bir bağlantı içerip içermediğini gösterir. Yalnızca hücre bir formül hücresi olduğunda geçerlidir. |
| [DateTimeValue](../../aspose.cells/cell/datetimevalue) { get; } | Hücrede bulunan DateTime değerini alır. |
| [DisplayStringValue](../../aspose.cells/cell/displaystringvalue) { get; } | Hücrenin görüntüleme stiline göre bu hücrenin biçimlendirilmiş dize değerini alır. |
| [DoubleValue](../../aspose.cells/cell/doublevalue) { get; } | Hücrede bulunan çift değeri alır. |
| [FloatValue](../../aspose.cells/cell/floatvalue) { get; } | Hücrede bulunan kayan nokta değerini alır. |
| [Formula](../../aspose.cells/cell/formula) { get; set; } | Şunun formülünü alır veya ayarlar:[`Cell`](../cell) . |
| [FormulaLocal](../../aspose.cells/cell/formulalocal) { get; set; } | Hücrenin yerel olarak biçimlendirilmiş formülünü alın. |
| [HtmlString](../../aspose.cells/cell/htmlstring) { get; set; } | Bu hücredeki verileri ve bazı biçimleri içeren html dizesini alır ve ayarlar. |
| [IntValue](../../aspose.cells/cell/intvalue) { get; } | Hücrede bulunan tamsayı değerini alır. |
| [IsArrayFormula](../../aspose.cells/cell/isarrayformula) { get; } | Hücre formülünün bir dizi formülü olup olmadığını gösterir. |
| [IsArrayHeader](../../aspose.cells/cell/isarrayheader) { get; } | Hücrenin formülünü ve dizi formülünü gösterir ve dizinin ilk hücresidir. |
| [IsErrorValue](../../aspose.cells/cell/iserrorvalue) { get; } | Bu hücrenin değerinin bir hata olup olmadığını kontrol eder. |
| [IsFormula](../../aspose.cells/cell/isformula) { get; } | Belirtilen hücrenin formül içerip içermediğini temsil eder. |
| [IsMerged](../../aspose.cells/cell/ismerged) { get; } | Bir hücrenin birleştirilmiş aralığın parçası olup olmadığını kontrol eder. |
| [IsNumericValue](../../aspose.cells/cell/isnumericvalue) { get; } | Bu hücrenin iç değerinin sayısal olup olmadığını gösterir(int, double ve datetime) |
| [IsSharedFormula](../../aspose.cells/cell/issharedformula) { get; } | Hücre formülünün paylaşılan formülün parçası olup olmadığını gösterir. |
| [IsStyleSet](../../aspose.cells/cell/isstyleset) { get; } | Hücrenin stilinin ayarlanıp ayarlanmadığını gösterir. false döndürürse, bu hücrenin varsayılan hücre biçimine sahip olduğu anlamına gelir. |
| [IsTableFormula](../../aspose.cells/cell/istableformula) { get; } | Bu hücrenin tablo formülünün parçası olup olmadığını gösterir. |
| [Name](../../aspose.cells/cell/name) { get; } | Hücrenin adını alır. |
| [NumberCategoryType](../../aspose.cells/cell/numbercategorytype) { get; } | Bu hücrenin sayı biçimlendirmesinin kategori türünü temsil eder. |
| [R1C1Formula](../../aspose.cells/cell/r1c1formula) { get; set; } | Şunun bir R1C1 formülünü alır veya ayarlar:[`Cell`](../cell) . |
| [Row](../../aspose.cells/cell/row) { get; } | Hücrenin satır numarasını (sıfır tabanlı) alır. |
| [SharedStyleIndex](../../aspose.cells/cell/sharedstyleindex) { get; } | Stil havuzunda hücrenin paylaşılan stil dizinini alır. |
| [StringValue](../../aspose.cells/cell/stringvalue) { get; } | Hücrede bulunan dize değerini alır. Bu hücrenin türü dize ise, dize değerinin kendisini döndürün. Diğer hücre türleri için, biçimlendirilmiş dize değeri (bu hücrenin belirtilen stiliyle biçimlendirilmiş) döndürülür. Biçimlendirilmiş hücre değeri, sizin belirlediğiniz değerle aynıdır. bir hücreyi metin olarak kopyalarken (örneğin, hücreyi metin düzenleyiciye kopyalamak veya csv'ye dışa aktarmak gibi). |
| [Type](../../aspose.cells/cell/type) { get; } | Hücre değeri türünü temsil eder. |
| [Value](../../aspose.cells/cell/value) { get; set; } | Bu hücrede bulunan değeri alır. |
| [Worksheet](../../aspose.cells/cell/worksheet) { get; } | Üst çalışma sayfasını alır. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [Calculate](../../aspose.cells/cell/calculate#calculate)(CalculationOptions) | Hücrenin formülünü hesaplar. |
| [Characters](../../aspose.cells/cell/characters)(int, int) | Hücre metni içinde bir dizi karakter temsil eden bir Karakterler nesnesi döndürür. |
| [Copy](../../aspose.cells/cell/copy)(Cell) | Verileri bir kaynak hücreden kopyalar. |
| [Equals](../../aspose.cells/cell/equals#equals)(Cell) | Bu nesnenin başka bir hücre nesnesiyle aynı hücreye başvurup göndermediğini kontrol eder. |
| override [Equals](../../aspose.cells/cell/equals#equals_1)(object) | Bu nesnenin başka bir hücreyle aynı hücreye başvurup göndermediğini kontrol eder. |
| [GetArrayRange](../../aspose.cells/cell/getarrayrange)() | Hücrenin formülü bir dizi formülü ise dizi aralığını alır. |
| [GetCharacters](../../aspose.cells/cell/getcharacters#getcharacters)() | Hücre metni içindeki bir karakter aralığını temsil eden tüm Karakterler nesnelerini döndürür. |
| [GetCharacters](../../aspose.cells/cell/getcharacters#getcharacters_1)(bool) | Hücre metni içindeki bir karakter aralığını temsil eden tüm Karakterler nesnelerini döndürür. |
| [GetConditionalFormattingResult](../../aspose.cells/cell/getconditionalformattingresult)() | Koşullu biçimlendirmenin sonucunu alın. |
| [GetDependents](../../aspose.cells/cell/getdependents)(bool) | Formülü bu hücreye doğrudan başvuran tüm hücreleri alın. |
| [GetDependentsInCalculation](../../aspose.cells/cell/getdependentsincalculation)(bool) | Hesaplanan sonucu bu hücreye bağlı olan tüm hücreleri alır. |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle#getdisplaystyle)() | Hücrenin görüntüleme stilini alır. Bu hücre, koşullu biçimlendirme, liste nesneleri vb. gibi diğer ayarlardan da etkilenirse, o zaman görüntüleme stili hücreden farklı olabilir.GetStyle(). |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle#getdisplaystyle_1)(bool) | Hücrenin görüntüleme stilini alır. Hücre koşullu biçimlendirilmişse, görüntüleme stili hücre ile aynı değildir.GetStyle(). |
| [GetFormatConditions](../../aspose.cells/cell/getformatconditions)() | Bu hücre için geçerli olan biçim koşullarını alır. |
| [GetFormula](../../aspose.cells/cell/getformula)(bool, bool) | Bu hücrenin formülünü alın. |
| override [GetHashCode](../../aspose.cells/cell/gethashcode)() | Belirli bir tür için karma işlevi işlevi görür. |
| [GetHeightOfValue](../../aspose.cells/cell/getheightofvalue)() | Değerin yüksekliğini piksel cinsinden alır. |
| [GetHtmlString](../../aspose.cells/cell/gethtmlstring)(bool) | Bu hücredeki verileri ve bazı biçimleri içeren html dizesini alır. |
| [GetMergedRange](../../aspose.cells/cell/getmergedrange)() | Bir döndürür[`Range`](../range) birleştirilmiş bir aralığı temsil eden nesne. |
| [GetPrecedents](../../aspose.cells/cell/getprecedents)() | Bu hücrenin formülünde görünen tüm başvuruları alır. |
| [GetPrecedentsInCalculation](../../aspose.cells/cell/getprecedentsincalculation)() | Bu hücre formülü tarafından hesaplanırken kullanılan tüm emsalleri (geçerli çalışma kitabındaki hücrelere başvuru) alır. |
| [GetStringValue](../../aspose.cells/cell/getstringvalue)(CellValueFormatStrategy) | Belirli biçimlendirilmiş stratejiye göre dize değerini alır. |
| [GetStyle](../../aspose.cells/cell/getstyle#getstyle)() | Hücre stilini alır. |
| [GetStyle](../../aspose.cells/cell/getstyle#getstyle_1)(bool) | checkBorders true ise, diğer hücrelerin sınırlarının bu hücrenin stilini etkileyip etkilemeyeceğini kontrol edin. |
| [GetTable](../../aspose.cells/cell/gettable)() | Bu hücreyi içeren tabloyu alır. |
| [GetValidation](../../aspose.cells/cell/getvalidation)() | Bu hücreye uygulanan doğrulamayı alır. |
| [GetValidationValue](../../aspose.cells/cell/getvalidationvalue)() | Bu hücreye uygulanan doğrulama değerini alır. |
| [GetWidthOfValue](../../aspose.cells/cell/getwidthofvalue)() | Değerin genişliğini piksel cinsinden alır. |
| [IsRichText](../../aspose.cells/cell/isrichtext)() | Hücre dizesi değerinin zengin bir metin olup olmadığını gösterir. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue)(bool) | Hücreye bir boole değeri koyar. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_3)(DateTime) | Hücreye bir DateTime değeri koyar. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_1)(double) | Hücreye bir çift değer koyar. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_2)(int) | Hücreye bir tamsayı değeri koyar. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_4)(object) | Hücreye bir nesne değeri koyar. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_5)(string) | Hücreye bir dize değeri koyar. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_6)(string, bool) | Hücreye bir dize değeri koyar ve uygunsa değeri başka bir veri türüne dönüştürür. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_7)(string, bool, bool) | Hücreye bir değer koyar, uygunsa değer başka bir veri tipine dönüştürülür ve hücrenin sayı formatı sıfırlanır. |
| [RemoveArrayFormula](../../aspose.cells/cell/removearrayformula)(bool) | Dizi formülünü kaldırın. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula#setarrayformula)(string, int, int) | Bir dizi formülü (ms excel olarak CTRL+SHIFT+ENTER ile girilen eski dizi formülü) bir hücre aralığına ayarlar. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula#setarrayformula_1)(string, int, int, FormulaParseOptions) | Bir dizi formülü bir hücre aralığına ayarlar. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula#setarrayformula_2)(string, int, int, FormulaParseOptions, object[][]) | Bir dizi formülü bir hücre aralığına ayarlar. |
| [SetCharacters](../../aspose.cells/cell/setcharacters)(FontSetting[]) | Hücrenin zengin metin biçimini ayarlar. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula#setdynamicarrayformula)(string, FormulaParseOptions, bool) | Dinamik dizi formülünü ayarlar ve mümkünse formülün komşu hücrelere dökülmesini sağlar. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula#setdynamicarrayformula_1)(string, FormulaParseOptions, object[][], bool, bool) | Dinamik dizi formülünü ayarlar ve mümkünse formülün komşu hücrelere dökülmesini sağlar. |
| [SetFormula](../../aspose.cells/cell/setformula#setformula_2)(string, object) | Formülü ve formülün değerini ayarlayın. |
| [SetFormula](../../aspose.cells/cell/setformula#setformula)(string, FormulaParseOptions, object) | Formülü ve formülün değerini ayarlayın. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula#setsharedformula)(string, int, int) | Bir hücre aralığına formül ayarlar. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula#setsharedformula_1)(string, int, int, FormulaParseOptions) | Bir hücre aralığına formül ayarlar. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula#setsharedformula_2)(string, int, int, FormulaParseOptions, object[][]) | Bir hücre aralığına formül ayarlar. |
| [SetStyle](../../aspose.cells/cell/setstyle#setstyle)(Style) | Hücre stilini ayarlar. |
| [SetStyle](../../aspose.cells/cell/setstyle#setstyle_2)(Style, bool) | Hücre stilini uygulayın. |
| [SetStyle](../../aspose.cells/cell/setstyle#setstyle_1)(Style, StyleFlag) | Hücre stilini uygulayın. |
| override [ToString](../../aspose.cells/cell/tostring)() | Geçerli Cell nesnesini temsil eden bir dize döndürür. |

### Örnekler

```csharp
[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

// Bir hücreye bir dize koy
Cell cell = cells[0, 0];
cell.PutValue("Hello");

string first = cell.StringValue;
	
// Bir hücreye bir tamsayı koyun
cell = cells["B1"];
cell.PutValue(12);

int second = cell.IntValue;

// Bir hücreye bir çift koy
cell = cells[0, 2];
cell.PutValue(-1.234);

double third = cell.DoubleValue;

//hücreye formül gir
cell = cells["D1"];
cell.Formula = "=B1 + C1";

//Birleştirilmiş bir formül koyun: "toplam(ortalama(b1,c1), b1)" b2'deki hücreye
cell = cells["b2"];
cell.Formula = "=sum(average(b1,c1), b1)";

// Bir hücrenin stilini ayarla
Style style = cell.GetStyle();
//Arka plan rengini ayarla
style.BackgroundColor = Color.Yellow;
// Bir hücrenin biçimini ayarla
style.Font.Name = "Courier New";
style.VerticalAlignment = TextAlignmentType.Top;
cell.SetStyle(style);



[Visual Basic]

Dim excel as Workbook = new Workbook()
Dim cells as Cells = exce.Worksheets(0).Cells

'Bir hücreye bir dize koyun
Dim cell as Cell = cells(0, 0)
cell.PutValue("Hello")

Dim first as String = cell.StringValue
	
// Bir hücreye bir tamsayı koyun
cell = cells("B1")
cell.PutValue(12)

Dim second as Integer = cell.IntValue

// Bir hücreye bir çift koy
cell = cells(0, 2)
cell.PutValue(-1.234)

Dim third as Double = cell.DoubleValue

//hücreye formül gir
cell = cells("D1")
cell.Formula = "=B1 + C1"

//Birleştirilmiş bir formül koyun: "toplam(ortalama(b1,c1), b1)" b2'deki hücreye
cell = cells("b2")
cell.Formula = "=sum(average(b1,c1), b1)"
	
// Bir hücrenin stilini ayarla
Dim style as Style = cell.GetStyle()

//Arka plan rengini ayarla
style.BackgroundColor = Color.Yellow
// Bir hücrenin yazı tipini ayarla
style.Font.Name = "Courier New"
style.VerticalAlignment = TextAlignmentType.Top
cell.SetStyle(style)
```

### Ayrıca bakınız

* ad alanı [Aspose.Cells](../../aspose.cells)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
