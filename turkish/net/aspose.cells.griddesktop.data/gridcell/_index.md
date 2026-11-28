---
title: "Sınıf GridCell"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridDesktop.Data.GridCell sınıfı. Bir hücre nesnesini temsil eder"
type: docs
url: /tr/net/aspose.cells.griddesktop.data/gridcell/
---
## GridCell class

Bir hücre nesnesini temsil eder.

```csharp
public class GridCell
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [BoolValue](../../aspose.cells.griddesktop.data/gridcell/boolvalue/) { get; } | Hücrede bulunan boolean değeri alır. |
| [Column](../../aspose.cells.griddesktop.data/gridcell/column/) { get; } | Hücrenin sütun numarasını (sıfır tabanlı) alır. |
| [DateValue](../../aspose.cells.griddesktop.data/gridcell/datevalue/) { get; } | Hücrede bulunan DateTime değerini alır. |
| [DisplayStringValue](../../aspose.cells.griddesktop.data/gridcell/displaystringvalue/) { get; } | Bu hücrenin biçimlendirilmiş dize değerini alır. |
| [DoubleValue](../../aspose.cells.griddesktop.data/gridcell/doublevalue/) { get; } | Hücrede bulunan double değerini alır. |
| [FloatValue](../../aspose.cells.griddesktop.data/gridcell/floatvalue/) { get; } | Hücrede bulunan float değerini alır. |
| [Formula](../../aspose.cells.griddesktop.data/gridcell/formula/) { get; set; } | Hücrenin formülünü alır veya ayarlar. |
| [HasCustomStyle](../../aspose.cells.griddesktop.data/gridcell/hascustomstyle/) { get; } | Bu hücrenin, ilgili satır, sütun veya çalışma kitabından devralınan varsayılan stilden farklı özel stil ayarlarına sahip olup olmadığını gösterir. |
| [HtmlString](../../aspose.cells.griddesktop.data/gridcell/htmlstring/) { get; set; } | Bu hücredeki veri ve bazı biçimlendirmeleri içeren html dizesini alır ve ayarlar. |
| [IntValue](../../aspose.cells.griddesktop.data/gridcell/intvalue/) { get; } | Hücrede bulunan tam sayı değerini alır. |
| [IsStyleSet](../../aspose.cells.griddesktop.data/gridcell/isstyleset/) { get; } | Hücrenin stilinin ayarlanıp ayarlanmadığını gösterir. False dönerse, bu hücrenin varsayılan hücre biçimine sahip olduğu anlamına gelir. |
| [Location](../../aspose.cells.griddesktop.data/gridcell/location/) { get; } |  |
| [Name](../../aspose.cells.griddesktop.data/gridcell/name/) { get; } | Hücrenin adını alır. Örneğin: A1, F102. |
| [Protected](../../aspose.cells.griddesktop.data/gridcell/protected/) { get; set; } | Hücrenin korumalı olup olmadığını gösterir. Değer "true" ise, kullanıcı kullanıcı arayüzü üzerinden hücreyi değiştiremez. Bu öznitelik Style.CellLocked özelliğiyle hiçbir ilişkisi yoktur ve ızgara verileri dışa aktarıldığında dosyaya kaydedilmez. Varsayılan değer "false"dır. |
| [Row](../../aspose.cells.griddesktop.data/gridcell/row/) { get; } | Hücrenin satır numarasını (sıfır tabanlı) alır. |
| [StringValue](../../aspose.cells.griddesktop.data/gridcell/stringvalue/) { get; } | Hücrede bulunan dize değerini alır. |
| [Style](../../aspose.cells.griddesktop.data/gridcell/style/) { get; set; } | Hücre stilinin bir kopyasını alır. Hücre için stili ayarlar. |
| [Type](../../aspose.cells.griddesktop.data/gridcell/type/) { get; } | hücre değer tipini döndürür, anlamı GridCellValueType.java dosyasından görülebilir |
| [Value](../../aspose.cells.griddesktop.data/gridcell/value/) { get; set; } | Bu hücrede bulunan değeri alır. |
| [Worksheet](../../aspose.cells.griddesktop.data/gridcell/worksheet/) { get; } | Çalışma sayfası nesnesini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [ContainsExternalLink](../../aspose.cells.griddesktop.data/gridcell/containsexternallink/)() | Bu hücrenin harici bir bağlantı içerip içermediğini gösterir. Yalnızca hücre bir formül hücresi olduğunda geçerlidir. |
| [Copy](../../aspose.cells.griddesktop.data/gridcell/copy/)(GridCell) | Bir kaynak hücreden verileri kopyalar. |
| [CopyStyle](../../aspose.cells.griddesktop.data/gridcell/copystyle/)(Style) | stili kopyalar ve hücre için stili ayarlar |
| override [Equals](../../aspose.cells.griddesktop.data/gridcell/equals/)(object) |  |
| [GetCellArea](../../aspose.cells.griddesktop.data/gridcell/getcellarea/)() |  |
| [GetFont](../../aspose.cells.griddesktop.data/gridcell/getfont/)() | Hücre yazı tipini alır. Yazı tipini değiştirdiğinizde, hücreye yazı tipini ayarlamak için "SetFont" metodunu çağırmalısınız. |
| [GetFontColor](../../aspose.cells.griddesktop.data/gridcell/getfontcolor/)() | Hücre yazı tipi rengini alır. Rengi değiştirdiğinizde, hücreye yazı tipi rengini ayarlamak için "SetFontColor" metodunu çağırmalısınız. |
| override [GetHashCode](../../aspose.cells.griddesktop.data/gridcell/gethashcode/)() |  |
| [GetStyle](../../aspose.cells.griddesktop.data/gridcell/getstyle/)() | Hücre stilini alır. Stili değiştirdiğinizde, hücreye stili ayarlamak için "SetStyle" metodunu çağırmalısınız. |
| [GetValidation](../../aspose.cells.griddesktop.data/gridcell/getvalidation/)() | Bu hücreye uygulanan doğrulamayı alır. Ayarlanmamışsa null döndürür. |
| [GetWidthOfValue](../../aspose.cells.griddesktop.data/gridcell/getwidthofvalue/)() | Değerin piksel birimindeki genişliğini alır. |
| [GetWorksheet](../../aspose.cells.griddesktop.data/gridcell/getworksheet/)() | Üst çalışma sayfasını alır. |
| [IsErrorValue](../../aspose.cells.griddesktop.data/gridcell/iserrorvalue/)() | Bir formülün sonucu doğru bir şekilde değerlendirebilir olup olmadığını kontrol eder. |
| [IsFormula](../../aspose.cells.griddesktop.data/gridcell/isformula/)() | Belirtilen hücrenin formül içerip içermediğini temsil eder. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue)(bool) | Hücreye bir mantıksal değer koyar. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_3)(DateTime) | Hücreye bir DateTime değeri koyar. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_1)(double) | Hücreye bir double değeri koyar. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_2)(int) | Hücreye bir int değeri koyar. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_4)(object) | Hücreye bir nesne değeri koyar. setValue(Object param_object) ile aynı. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_5)(string) | Hücreye bir String değeri koyar. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_6)(string, bool) | Hücreye bir dize değeri koyar ve uygun olduğunda değeri başka bir veri tipine dönüştürür. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_7)(string, bool, bool) | Hücreye bir değer koyar, uygun olduğunda değer başka bir veri tipine dönüştürülür ve hücrenin sayı biçimi sıfırlanır. |
| [PutValueAndSetFormatByValue](../../aspose.cells.griddesktop.data/gridcell/putvalueandsetformatbyvalue/)(string) | Hücrenin değerini bir dize değeriyle ayarlar ve hücre biçimini bu değerle belirler. |
| [SetCellValue](../../aspose.cells.griddesktop.data/gridcell/setcellvalue/)(object) | Değer bir formül ise, bu yöntem hücrenin değerini FormulaType olarak ayarlar, |
| [SetCustom](../../aspose.cells.griddesktop.data/gridcell/setcustom/)(string) | özel biçimi ayarlar, null veya boş dize özel biçim olmadığı anlamına gelir. |
| [SetFont](../../aspose.cells.griddesktop.data/gridcell/setfont/)(Font) | Hücreye yazı tipini ayarlar. Performansı artırmak için "SetFont" yöntemini uygulayın, "Font" özelliğini uygulamayın. |
| [SetFontColor](../../aspose.cells.griddesktop.data/gridcell/setfontcolor/)(Color) | Hücreye yazı tipi rengini ayarlar. Performansı artırmak için "SetFontColor" yöntemini uygulayın, "FontColor" özelliğini uygulamayın. |
| [SetFormula](../../aspose.cells.griddesktop.data/gridcell/setformula/)(string, object) | Formülü ve formülün değerini ayarlayın. |
| [SetNumberType](../../aspose.cells.griddesktop.data/gridcell/setnumbertype/)(int) | Sayıların ve tarihlerin görüntüleme biçimini ayarlayın. |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcell/setstyle/)(Style) | Hücreye stili ayarlar. Performansı artırmak için "SetStyle" yöntemini uygulayın, "Style" özelliğini uygulamayın. |
| override [ToString](../../aspose.cells.griddesktop.data/gridcell/tostring/)() | Geçerli Cell nesnesini temsil eden bir dize döndürür. |
| [operator ==](../../aspose.cells.griddesktop.data/gridcell/op_equality/) |  |
| [operator !=](../../aspose.cells.griddesktop.data/gridcell/op_inequality/) |  |

### Ayrıca Bakınız

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


