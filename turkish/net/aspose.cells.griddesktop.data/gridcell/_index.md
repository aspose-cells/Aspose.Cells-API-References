---
title: GridCell
second_title: Aspose.Cells for .NET API Referansı
description: Bir hücre nesnesini temsil eder.
type: docs
weight: 370
url: /tr/net/aspose.cells.griddesktop.data/gridcell/
---
## GridCell class

Bir hücre nesnesini temsil eder.

```csharp
public class GridCell
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [BoolValue](../../aspose.cells.griddesktop.data/gridcell/boolvalue) { get; } | Hücrede bulunan boole değerini alır. |
| [Column](../../aspose.cells.griddesktop.data/gridcell/column) { get; } | Hücrenin sütun numarasını (sıfır tabanlı) alır. |
| [DateValue](../../aspose.cells.griddesktop.data/gridcell/datevalue) { get; } | Hücrede bulunan DateTime değerini alır. |
| [DisplayStringValue](../../aspose.cells.griddesktop.data/gridcell/displaystringvalue) { get; } | Bu hücrenin biçimlendirilmiş dize değerini alır. |
| [DoubleValue](../../aspose.cells.griddesktop.data/gridcell/doublevalue) { get; } | Hücrede bulunan çift değeri alır. |
| [FloatValue](../../aspose.cells.griddesktop.data/gridcell/floatvalue) { get; } | Hücrede bulunan kayan nokta değerini alır. |
| [Formula](../../aspose.cells.griddesktop.data/gridcell/formula) { get; set; } | Şunun formülünü alır veya ayarlar:Cell . |
| [HtmlString](../../aspose.cells.griddesktop.data/gridcell/htmlstring) { get; set; } | Bu hücredeki verileri ve bazı biçimlendirmeleri içeren html dizesini alır ve ayarlar. |
| [IntValue](../../aspose.cells.griddesktop.data/gridcell/intvalue) { get; } | Hücrede bulunan tamsayı değerini alır. |
| [IsStyleSet](../../aspose.cells.griddesktop.data/gridcell/isstyleset) { get; } | Hücrenin stilinin ayarlanıp ayarlanmadığını gösterir. false döndürürse, bu hücrenin varsayılan hücre biçimine sahip olduğu anlamına gelir. |
| [Location](../../aspose.cells.griddesktop.data/gridcell/location) { get; } |  |
| [Name](../../aspose.cells.griddesktop.data/gridcell/name) { get; } | Hücrenin adını alır. Örneğin: A1, F102. |
| [Protected](../../aspose.cells.griddesktop.data/gridcell/protected) { get; set; } | Hücrenin korunup korunmadığını gösterir. Değer "true" ise, kullanıcı hücreyi kullanıcı arabirimi aracılığıyla değiştiremez. Bu özniteliğin Style.CellLocked özelliği ile ilgisi yoktur ve şu durumlarda dosyaya kaydedilmez: ızgara verileri dışa aktarıldı. Varsayılan değer "false"dır. |
| [Row](../../aspose.cells.griddesktop.data/gridcell/row) { get; } | Hücrenin satır numarasını (sıfır tabanlı) alır. |
| [StringValue](../../aspose.cells.griddesktop.data/gridcell/stringvalue) { get; } | Hücrede bulunan dize değerini alır. |
| [Style](../../aspose.cells.griddesktop.data/gridcell/style) { get; set; } | Hücre stilinin kopyasını alır. hücrenin stilini ayarlayın. |
| [Type](../../aspose.cells.griddesktop.data/gridcell/type) { get; } | hücre değeri türünü döndürür, anlamı GridCellValueType.java görebilir |
| [Value](../../aspose.cells.griddesktop.data/gridcell/value) { get; set; } | Bu hücrede bulunan değeri alır. |
| [Worksheet](../../aspose.cells.griddesktop.data/gridcell/worksheet) { get; } | Çalışma sayfası nesnesini alır. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [ContainsExternalLink](../../aspose.cells.griddesktop.data/gridcell/containsexternallink)() | Bu hücrenin harici bir bağlantı içerip içermediğini gösterir. Yalnızca hücre bir formül hücresi olduğunda geçerlidir. |
| [Copy](../../aspose.cells.griddesktop.data/gridcell/copy)(GridCell) | Verileri bir kaynak hücreden kopyalar. |
| [CopyStyle](../../aspose.cells.griddesktop.data/gridcell/copystyle)(Style) | stili kopyalayın ve hücrenin stilini ayarlayın |
| override [Equals](../../aspose.cells.griddesktop.data/gridcell/equals)(object) |  |
| [GetCellArea](../../aspose.cells.griddesktop.data/gridcell/getcellarea)() |  |
| [GetFont](../../aspose.cells.griddesktop.data/gridcell/getfont)() | Hücre yazı tipini alır. Yazı tipini değiştirirken, yazı tipini hücreye ayarlamak için "SetFont" yöntemini, çağırmalısınız. |
| [GetFontColor](../../aspose.cells.griddesktop.data/gridcell/getfontcolor)() | Hücre yazı tipi rengini alır. Rengi değiştirirken, yazı tipi rengini hücreye ayarlamak için "SetFontColor" yöntemini, çağırmalısınız. |
| override [GetHashCode](../../aspose.cells.griddesktop.data/gridcell/gethashcode)() |  |
| [GetStyle](../../aspose.cells.griddesktop.data/gridcell/getstyle)() | Hücre stilini alır. Stili değiştirirken, stili hücreye ayarlamak için "SetStyle" yöntemini, çağırmalısınız. |
| [GetValidation](../../aspose.cells.griddesktop.data/gridcell/getvalidation)() | Bu hücreye uygulanan doğrulamayı alır. |
| [GetWidthOfValue](../../aspose.cells.griddesktop.data/gridcell/getwidthofvalue)() | Değerin genişliğini piksel cinsinden alır. |
| [GetWorksheet](../../aspose.cells.griddesktop.data/gridcell/getworksheet)() | Üst çalışma sayfasını alır. |
| [IsErrorValue](../../aspose.cells.griddesktop.data/gridcell/iserrorvalue)() | Bir formülün bir sonucu doğru şekilde değerlendirip değerlendiremeyeceğini kontrol eder. |
| [IsFormula](../../aspose.cells.griddesktop.data/gridcell/isformula)() | Belirtilen hücrenin formül içerip içermediğini temsil eder. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue)(bool) | Hücreye bir boole değeri koyar. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_3)(DateTime) | Hücreye bir DateTime değeri koyar. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_1)(double) | Hücreye bir çift değer koyar. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_2)(int) | Hücreye bir int değeri koyar. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_4)(object) | setValue(Object param_object) ile aynı hücreye bir nesne değeri koyar |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_5)(string) | Hücreye bir Dize değeri koyar. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_6)(string, bool) | Hücreye bir dize değeri koyar ve uygunsa değeri başka bir veri türüne dönüştürür. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_7)(string, bool, bool) | Hücreye bir değer koyar, uygunsa değer başka bir veri tipine dönüştürülür ve hücrenin sayı formatı sıfırlanır. |
| [PutValueAndSetFormatByValue](../../aspose.cells.griddesktop.data/gridcell/putvalueandsetformatbyvalue)(string) | Hücrenin değerini bir dize değeriyle ayarlar ve hücre biçimini bu değerle ayarlar. |
| [SetCellValue](../../aspose.cells.griddesktop.data/gridcell/setcellvalue)(object) | Değer bir formülse, bu yöntem hücrenin değerini FormulaType, olarak ayarlar. |
| [SetCustom](../../aspose.cells.griddesktop.data/gridcell/setcustom)(string) | özel biçimi ayarlar, boş veya boş dize, özel biçim olmadığı anlamına gelir. |
| [SetFont](../../aspose.cells.griddesktop.data/gridcell/setfont)(Font) | Yazı tipini hücreye ayarlar. Performansı artırmak için "SetFont" yöntemini uygulayın, "Font" özelliğini uygulamayın. |
| [SetFontColor](../../aspose.cells.griddesktop.data/gridcell/setfontcolor)(Color) | Yazı tipi rengini hücreye ayarlar. Performansı artırmak için "SetFontColor" yöntemini uygulayın, "FontColor" özelliğini uygulamayın. |
| [SetFormula](../../aspose.cells.griddesktop.data/gridcell/setformula)(string, object) | Formülü ve formülün değerini ayarlayın. |
| [SetNumberType](../../aspose.cells.griddesktop.data/gridcell/setnumbertype)(int) | sayıların ve tarihlerin görüntülenme biçimini ayarlayın |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcell/setstyle)(Style) | Stili hücreye ayarlar. Performansı artırmak için "SetStyle" yöntemini uygulayın, "Style" özelliğini uygulamayın. |
| [ToString](../../aspose.cells.griddesktop.data/gridcell/tostring#tostring)() | Geçerli Cell nesnesini temsil eden bir dize döndürür. |
| [operator ==](../../aspose.cells.griddesktop.data/gridcell/op_equality) |  |
| [operator !=](../../aspose.cells.griddesktop.data/gridcell/op_inequality) |  |

### Ayrıca bakınız

* ad alanı [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data)
* toplantı [Aspose.Cells.GridDesktop](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
