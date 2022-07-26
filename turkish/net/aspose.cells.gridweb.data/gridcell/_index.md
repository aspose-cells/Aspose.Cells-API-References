---
title: GridCell
second_title: Aspose.Cells for .NET API Referansı
description: Bir hücre nesnesini temsil eder.
type: docs
weight: 150
url: /tr/net/aspose.cells.gridweb.data/gridcell/
---
## GridCell class

Bir hücre nesnesini temsil eder.

```csharp
public class GridCell
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [BoolValue](../../aspose.cells.gridweb.data/gridcell/boolvalue) { get; } | Hücrede bulunan boole değerini alır. |
| [Column](../../aspose.cells.gridweb.data/gridcell/column) { get; } | Hücrenin sütun numarasını (sıfır tabanlı) alır. |
| [DateValue](../../aspose.cells.gridweb.data/gridcell/datevalue) { get; } | Hücrede bulunan DateTime değerini alır. |
| [DisplayStringValue](../../aspose.cells.gridweb.data/gridcell/displaystringvalue) { get; } | Bu hücrenin biçimlendirilmiş dize değerini alır. |
| [DoubleValue](../../aspose.cells.gridweb.data/gridcell/doublevalue) { get; } | Hücrede bulunan çift değeri alır. |
| [FloatValue](../../aspose.cells.gridweb.data/gridcell/floatvalue) { get; } | Hücrede bulunan kayan nokta değerini alır. |
| [Formula](../../aspose.cells.gridweb.data/gridcell/formula) { get; set; } | Şunun formülünü alır veya ayarlar:Cell . |
| [HtmlString](../../aspose.cells.gridweb.data/gridcell/htmlstring) { get; set; } | Bu hücredeki verileri ve bazı biçimlendirmeleri içeren html dizesini alır ve ayarlar. |
| [IntValue](../../aspose.cells.gridweb.data/gridcell/intvalue) { get; } | Hücrede bulunan tamsayı değerini alır. |
| [IsStyleSet](../../aspose.cells.gridweb.data/gridcell/isstyleset) { get; } | Hücrenin stilinin ayarlanıp ayarlanmadığını gösterir. false döndürürse, bu hücrenin varsayılan hücre biçimine sahip olduğu anlamına gelir. |
| [Name](../../aspose.cells.gridweb.data/gridcell/name) { get; } | Hücrenin adını alır. Örneğin: A1, F102. |
| [Row](../../aspose.cells.gridweb.data/gridcell/row) { get; } | Hücrenin satır numarasını (sıfır tabanlı) alır. |
| [StringValue](../../aspose.cells.gridweb.data/gridcell/stringvalue) { get; } | Hücrede bulunan dize değerini alır. |
| [Style](../../aspose.cells.gridweb.data/gridcell/style) { get; set; } | Hücre stilinin kopyasını alır. hücrenin stilini ayarlayın. |
| [Type](../../aspose.cells.gridweb.data/gridcell/type) { get; } | hücre değeri türünü döndürür, anlamı GridCellValueType.java görebilir |
| [Value](../../aspose.cells.gridweb.data/gridcell/value) { get; set; } | Bu hücrede bulunan değeri alır. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [ContainsExternalLink](../../aspose.cells.gridweb.data/gridcell/containsexternallink)() | Bu hücrenin harici bir bağlantı içerip içermediğini gösterir. Yalnızca hücre bir formül hücresi olduğunda geçerlidir. |
| [Copy](../../aspose.cells.gridweb.data/gridcell/copy)(GridCell) | Verileri bir kaynak hücreden kopyalar. |
| [CopyStyle](../../aspose.cells.gridweb.data/gridcell/copystyle)(GridTableItemStyle) | stili kopyalayın ve hücrenin stilini ayarlayın |
| [CreateComment](../../aspose.cells.gridweb.data/gridcell/createcomment)(string, string, bool) | Bir hücre için bir yorum nesnesi oluşturur. |
| [CreateValidation](../../aspose.cells.gridweb.data/gridcell/createvalidation)(GridValidationType, bool) | Bir hücre için bir doğrulama nesnesi oluşturur. |
| override [Equals](../../aspose.cells.gridweb.data/gridcell/equals)(object) |  |
| [GetCellArea](../../aspose.cells.gridweb.data/gridcell/getcellarea)() |  |
| [GetComment](../../aspose.cells.gridweb.data/gridcell/getcomment)() | Bu hücrede yorum nesnesi al |
| override [GetHashCode](../../aspose.cells.gridweb.data/gridcell/gethashcode)() |  |
| [GetWidthOfValue](../../aspose.cells.gridweb.data/gridcell/getwidthofvalue)() | Değerin genişliğini piksel cinsinden alır. |
| [IsErrorValue](../../aspose.cells.gridweb.data/gridcell/iserrorvalue)() | Bir formülün bir sonucu doğru şekilde değerlendirip değerlendiremeyeceğini kontrol eder. |
| [IsFormula](../../aspose.cells.gridweb.data/gridcell/isformula)() | Belirtilen hücrenin formül içerip içermediğini temsil eder. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue)(bool) | Hücreye bir boole değeri koyar. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_3)(DateTime) | Hücreye bir DateTime değeri koyar. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_1)(double) | Hücreye bir çift değer koyar. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_2)(int) | Hücreye bir int değeri koyar. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_4)(object) | setValue(Object param_object) ile aynı hücreye bir nesne değeri koyar |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_5)(string) | Hücreye bir Dize değeri koyar. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_6)(string, bool) | Hücreye bir dize değeri koyar ve uygunsa değeri başka bir veri türüne dönüştürür. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_7)(string, bool, bool) | Hücreye bir değer koyar, uygunsa değer başka bir veri tipine dönüştürülür ve hücrenin sayı formatı sıfırlanır. |
| [PutValueAndSetFormatByValue](../../aspose.cells.gridweb.data/gridcell/putvalueandsetformatbyvalue)(string) | Hücrenin değerini bir dize değeriyle ayarlar ve hücre biçimini bu değerle ayarlar. |
| [RemoveComment](../../aspose.cells.gridweb.data/gridcell/removecomment)() | Hücrenin yorum nesnesini kaldırır. |
| [RemoveValidation](../../aspose.cells.gridweb.data/gridcell/removevalidation)() | Hücrenin doğrulama nesnesini kaldırır. |
| [SetBorder](../../aspose.cells.gridweb.data/gridcell/setborder)(WebBorderStyle) | Bir hücre için kenarlıklar (üst, alt, sol ve sağ) ayarlar, tüm kenarlıklar aynı kenarlık stiline sahiptir. |
| [SetCustom](../../aspose.cells.gridweb.data/gridcell/setcustom)(string) | özel biçimi ayarlar, boş veya boş dize, özel biçim olmadığı anlamına gelir. |
| [SetFormula](../../aspose.cells.gridweb.data/gridcell/setformula)(string, object) | Formülü ve formülün değerini ayarlayın. |
| [SetNumberType](../../aspose.cells.gridweb.data/gridcell/setnumbertype)(int) | sayıların ve tarihlerin görüntülenme biçimini ayarlayın |
| [ToString](../../aspose.cells.gridweb.data/gridcell/tostring#tostring)() | Geçerli Cell nesnesini temsil eden bir dize döndürür. |
| [operator ==](../../aspose.cells.gridweb.data/gridcell/op_equality) |  |
| [operator !=](../../aspose.cells.gridweb.data/gridcell/op_inequality) |  |

### Ayrıca bakınız

* ad alanı [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data)
* toplantı [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
