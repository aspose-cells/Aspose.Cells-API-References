---
title: "Sınıf GridCell"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridWeb.Data.GridCell sınıfı. Bir hücre nesnesini temsil eder."
type: docs
url: /tr/net/aspose.cells.gridweb.data/gridcell/
---
## GridCell class

Bir hücre nesnesini temsil eder.

```csharp
public class GridCell
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [BoolValue](../../aspose.cells.gridweb.data/gridcell/boolvalue/) { get; } | Hücrede bulunan boolean değeri alır. |
| [Column](../../aspose.cells.gridweb.data/gridcell/column/) { get; } | Hücrenin sütun numarasını (sıfır tabanlı) alır. |
| [DateValue](../../aspose.cells.gridweb.data/gridcell/datevalue/) { get; } | Hücrede bulunan DateTime değerini alır. |
| [DisplayStringValue](../../aspose.cells.gridweb.data/gridcell/displaystringvalue/) { get; } | Bu hücrenin biçimlendirilmiş dize değerini alır. |
| [DoubleValue](../../aspose.cells.gridweb.data/gridcell/doublevalue/) { get; } | Hücrede bulunan double değerini alır. |
| [FloatValue](../../aspose.cells.gridweb.data/gridcell/floatvalue/) { get; } | Hücrede bulunan float değerini alır. |
| [Formula](../../aspose.cells.gridweb.data/gridcell/formula/) { get; set; } | `GridCell`'in bir formülünü alır veya ayarlar. |
| [HtmlString](../../aspose.cells.gridweb.data/gridcell/htmlstring/) { get; set; } | Bu hücredeki veri ve bazı biçimlendirmeleri içeren html dizesini alır ve ayarlar. |
| [IntValue](../../aspose.cells.gridweb.data/gridcell/intvalue/) { get; } | Hücrede bulunan tam sayı değerini alır. |
| [IsStyleSet](../../aspose.cells.gridweb.data/gridcell/isstyleset/) { get; } | Hücrenin stilinin ayarlanıp ayarlanmadığını gösterir. False dönerse, bu hücrenin varsayılan hücre biçimine sahip olduğu anlamına gelir. |
| [Name](../../aspose.cells.gridweb.data/gridcell/name/) { get; } | Hücrenin adını alır. Örneğin: A1, F102. |
| [Row](../../aspose.cells.gridweb.data/gridcell/row/) { get; } | Hücrenin satır numarasını (sıfır tabanlı) alır. |
| [StringValue](../../aspose.cells.gridweb.data/gridcell/stringvalue/) { get; } | Hücrede bulunan dize değerini alır. |
| [Style](../../aspose.cells.gridweb.data/gridcell/style/) { get; set; } | Hücre stilinin bir kopyasını alır. Hücre için stili ayarlar. |
| [Type](../../aspose.cells.gridweb.data/gridcell/type/) { get; } | hücre değer tipini döndürür, anlamı GridCellValueType.java dosyasından görülebilir |
| [Value](../../aspose.cells.gridweb.data/gridcell/value/) { get; set; } | Bu hücrede bulunan değeri alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [ContainsExternalLink](../../aspose.cells.gridweb.data/gridcell/containsexternallink/)() | Bu hücrenin harici bir bağlantı içerip içermediğini gösterir. Yalnızca hücre bir formül hücresi olduğunda geçerlidir. |
| [Copy](../../aspose.cells.gridweb.data/gridcell/copy/)(GridCell) | Bir kaynak hücreden verileri kopyalar. |
| [CopyStyle](../../aspose.cells.gridweb.data/gridcell/copystyle/)(GridTableItemStyle) | stili kopyalar ve hücre için stili ayarlar |
| [CreateComment](../../aspose.cells.gridweb.data/gridcell/createcomment/)(string, string, bool) | Bir hücre için yorum nesnesi oluşturur. |
| [CreateValidation](../../aspose.cells.gridweb.data/gridcell/createvalidation/)(GridValidationType, bool) | Bir hücre için doğrulama nesnesi oluşturur. |
| override [Equals](../../aspose.cells.gridweb.data/gridcell/equals/)(object) | Bu nesnenin aynı hücreye başka bir hücre nesnesiyle referans verip vermediğini kontrol eder. |
| [GetComment](../../aspose.cells.gridweb.data/gridcell/getcomment/)() | Bu hücredeki yorum nesnesini al. |
| override [GetHashCode](../../aspose.cells.gridweb.data/gridcell/gethashcode/)() | Belirli bir tip için hash işlevi olarak hizmet eder. |
| [GetWidthOfValue](../../aspose.cells.gridweb.data/gridcell/getwidthofvalue/)() | Değerin piksel birimindeki genişliğini alır. |
| [IsErrorValue](../../aspose.cells.gridweb.data/gridcell/iserrorvalue/)() | Bir formülün sonucu doğru bir şekilde değerlendirebilir olup olmadığını kontrol eder. |
| [IsFormula](../../aspose.cells.gridweb.data/gridcell/isformula/)() | Belirtilen hücrenin formül içerip içermediğini temsil eder. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue)(bool) | Hücreye bir mantıksal değer koyar. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_3)(DateTime) | Hücreye bir DateTime değeri koyar. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_1)(double) | Hücreye bir double değeri koyar. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_2)(int) | Hücreye bir int değeri koyar. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_4)(object) | Hücreye bir nesne değeri koyar. setValue(Object param_object) ile aynı. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_5)(string) | Hücreye bir String değeri koyar. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_6)(string, bool) | Hücreye bir dize değeri koyar ve uygun olduğunda değeri başka bir veri tipine dönüştürür. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_7)(string, bool, bool) | Hücreye bir değer koyar, uygun olduğunda değer başka bir veri tipine dönüştürülür ve hücrenin sayı biçimi sıfırlanır. |
| [PutValueAndSetFormatByValue](../../aspose.cells.gridweb.data/gridcell/putvalueandsetformatbyvalue/)(string) | Hücrenin değerini bir dize değeriyle ayarlar ve hücre biçimini bu değerle belirler. |
| [RemoveComment](../../aspose.cells.gridweb.data/gridcell/removecomment/)() | Hücrenin yorum nesnesini kaldırır. |
| [RemoveValidation](../../aspose.cells.gridweb.data/gridcell/removevalidation/)() | Hücrenin doğrulama nesnesini kaldırır. |
| [SetBorder](../../aspose.cells.gridweb.data/gridcell/setborder/)(WebBorderStyle) | Bir hücre için kenarlıkları (üst, alt, sol ve sağ) ayarlar, tüm kenarlıkların aynı kenarlık stiline sahip olması. |
| [SetCustom](../../aspose.cells.gridweb.data/gridcell/setcustom/)(string) | özel biçimi ayarlar, null veya boş dize özel biçim olmadığı anlamına gelir. |
| [SetFormula](../../aspose.cells.gridweb.data/gridcell/setformula/)(string, object) | Formülü ve formülün değerini ayarlayın. |
| [SetNumberType](../../aspose.cells.gridweb.data/gridcell/setnumbertype/)(int) | Sayıların ve tarihlerin görüntüleme biçimini ayarlayın. |
| [ToString](../../aspose.cells.gridweb.data/gridcell/tostring/#tostring)() | Geçerli Cell nesnesini temsil eden bir dize döndürür. |
| [operator ==](../../aspose.cells.gridweb.data/gridcell/op_equality/) |  |
| [operator !=](../../aspose.cells.gridweb.data/gridcell/op_inequality/) |  |

### Ayrıca Bakınız

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


