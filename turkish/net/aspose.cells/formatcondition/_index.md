---
title: FormatCondition
second_title: Aspose.Cells for .NET API Referansı
description: Koşullu biçimlendirme koşulunu temsil eder.
type: docs
weight: 3560
url: /tr/net/aspose.cells/formatcondition/
---
## FormatCondition class

Koşullu biçimlendirme koşulunu temsil eder.

```csharp
public class FormatCondition
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [AboveAverage](../../aspose.cells/formatcondition/aboveaverage) { get; } | Koşullu biçimlendirmenin "AboveAverage" örneğini alın. Varsayılan örneğin kuralı, aralıktaki tüm değerler için ortalamanın üzerinde olan hücreleri vurgular. Yalnızca type = AboveAverage. için geçerlidir. |
| [ColorScale](../../aspose.cells/formatcondition/colorscale) { get; } | Koşullu biçimlendirmenin "ColorScale" örneğini alın. Varsayılan örnek bir "yeşil-sarı-kırmızı"dır 3ColorScale . Yalnızca type = ColorScale. için geçerlidir |
| [DataBar](../../aspose.cells/formatcondition/databar) { get; } | Koşullu biçimlendirmenin "DataBar" örneğini alın. Varsayılan örneğin rengi mavidir. Yalnızca şu tür için geçerlidir: DataBar. |
| [Formula1](../../aspose.cells/formatcondition/formula1) { get; set; } | Koşullu biçimlendirmeyle ilişkili değeri veya ifadeyi alır ve ayarlar. |
| [Formula2](../../aspose.cells/formatcondition/formula2) { get; set; } | Koşullu biçimlendirmeyle ilişkili değeri veya ifadeyi alır ve ayarlar. |
| [IconSet](../../aspose.cells/formatcondition/iconset) { get; } | Koşullu biçimlendirmenin "IconSet" örneğini alın. Varsayılan örneğin IconSetType'ı TrafficLights31. Yalnızca tür için geçerlidir = IconSet. |
| [Operator](../../aspose.cells/formatcondition/operator) { get; set; } | Koşullu biçim işleç türünü alır ve ayarlar. |
| [Priority](../../aspose.cells/formatcondition/priority) { get; set; } | Bu koşullu biçimlendirme kuralının önceliği. Bu değer, hangi biçiminin değerlendirilmesi ve işlenmesi gerektiğini belirlemek için kullanılır. Daha düşük sayısal değerler, '1' en yüksek öncelik olmak üzere, daha yüksek sayısal değerlerden daha yüksek önceliğe sahiptir. |
| [StopIfTrue](../../aspose.cells/formatcondition/stopiftrue) { get; set; } | Doğru, bu kural doğru olarak değerlendirildiğinde, bu kurala daha düşük önceliğe sahip hiçbir kural uygulanamaz. Yalnızca Excel 2007 için geçerlidir; |
| [Style](../../aspose.cells/formatcondition/style) { get; set; } | Koşullu biçimlendirilmiş hücre aralıklarının stilini alır veya ayarlar. |
| [Text](../../aspose.cells/formatcondition/text) { get; set; } | "Metin içerir" koşullu biçimlendirme kuralındaki metin değeri. Yalnızca tür için geçerlidir = includeText, notContainsText, beginWith ve endWith. Varsayılan değer null. |
| [TimePeriod](../../aspose.cells/formatcondition/timeperiod) { get; set; } | Bir "tarih meydana geliyor..." koşullu biçimlendirme kuralındaki geçerli zaman aralığı. Yalnızca tür için geçerlidir = timePeriod. Varsayılan değer TimePeriodType.Today. |
| [Top10](../../aspose.cells/formatcondition/top10) { get; } | Koşullu biçimlendirmenin "İlk 10" örneğini alın. Varsayılan örneğin kuralı, değerleri ilk 10 parantez içine giren hücreleri vurgular. Yalnızca tür için geçerlidir: Top10. |
| [Type](../../aspose.cells/formatcondition/type) { get; set; } | Koşullu biçimin Type. olup olmadığını alır ve ayarlar |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1#getformula1)(bool, bool) | Bu biçim koşuluyla ilişkili değeri veya ifadeyi alır. |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1#getformula1_2)(int, int) | Hücrenin koşullu biçimlendirmesinin formülünü alır. |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1#getformula1_1)(bool, bool, int, int) | Hücrenin koşullu biçimlendirmesinin değerini veya ifadesini alır. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2#getformula2)(bool, bool) | Bu biçim koşuluyla ilişkili değeri veya ifadeyi alır. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2#getformula2_2)(int, int) | Hücrenin koşullu biçimlendirmesinin formülünü alır. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2#getformula2_1)(bool, bool, int, int) | Hücrenin koşullu biçimlendirmesinin değerini veya ifadesini alır. |
| [SetFormula1](../../aspose.cells/formatcondition/setformula1)(string, bool, bool) | Bu biçim koşuluyla ilişkili değeri veya ifadeyi ayarlar. |
| [SetFormula2](../../aspose.cells/formatcondition/setformula2)(string, bool, bool) | Bu biçim koşuluyla ilişkili değeri veya ifadeyi ayarlar. |
| [SetFormulas](../../aspose.cells/formatcondition/setformulas)(string, string, bool, bool) | Bu biçim koşuluyla ilişkili değeri veya ifadeyi ayarlar. |

### Örnekler

```csharp

[C#]
//Bir Çalışma Kitabı nesnesini başlatma
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
 
//Boş bir koşullu biçimlendirme ekler
int index = sheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
 
//Koşullu biçim aralığını ayarlar.
CellArea ca = new CellArea();
ca.StartRow = 0;
ca.EndRow = 0;
ca.StartColumn = 0;
ca.EndColumn = 0;
fcs.AddArea(ca);
 
ca = new CellArea();
ca.StartRow = 1;
ca.EndRow = 1;
ca.StartColumn = 1;
ca.EndColumn = 1;
fcs.AddArea(ca);
 
//Koşul ekler.
int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");
 
//Koşul ekler.
int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");
 
//Arka plan rengini ayarlar.
FormatCondition fc = fcs[conditionIndex];
fc.Style.BackgroundColor = Color.Red;
 
//Excel dosyasını kaydetme
workbook.Save("output.xls");

[VB.NET]

'Bir Çalışma Kitabı nesnesini başlatma
Dim workbook As Workbook = New Workbook()
Dim sheet As Worksheet = workbook.Worksheets(0)
 
' Boş bir koşullu biçimlendirme ekler
Dim index As Integer = sheet.ConditionalFormattings.Add()
Dim fcs As FormatConditionCollection = sheet.ConditionalFormattings(index)
 
'Koşullu biçim aralığını ayarlar.
Dim ca As CellArea = New CellArea()
ca.StartRow = 0
ca.EndRow = 0
ca.StartColumn = 0
ca.EndColumn = 0
fcs.AddArea(ca)
ca = New CellArea()
ca.StartRow = 1
ca.EndRow = 1
ca.StartColumn = 1
ca.EndColumn = 1
fcs.AddArea(ca)
 
'Koşul ekler.
Dim conditionIndex As Integer = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100")
 
'Koşul ekler.
Dim conditionIndex2 As Integer = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100")
 
'Arka plan rengini ayarlar.
Dim fc As FormatCondition = fcs(conditionIndex)
fc.Style.BackgroundColor = Color.Red
 
'Excel dosyasını kaydetme
workbook.Save("output.xls")
```

### Ayrıca bakınız

* ad alanı [Aspose.Cells](../../aspose.cells)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
