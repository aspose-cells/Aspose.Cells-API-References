---
title: DataBar
second_title: Aspose.Cells for .NET API Referansı
description: DataBar koşullu biçimlendirme kuralını açıklayın. Bu koşullu biçimlendirme kuralı hücre aralığında derecelendirilmiş bir veri çubuğu görüntüler.
type: docs
weight: 1240
url: /tr/net/aspose.cells/databar/
---
## DataBar class

DataBar koşullu biçimlendirme kuralını açıklayın. Bu koşullu biçimlendirme kuralı, hücre aralığında derecelendirilmiş bir veri çubuğu görüntüler.

```csharp
public class DataBar
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [AxisColor](../../aspose.cells/databar/axiscolor) { get; set; } | Veri çubukları olarak koşullu biçimlendirmeye sahip hücreler için eksen rengini alır. |
| [AxisPosition](../../aspose.cells/databar/axisposition) { get; set; } | Koşullu biçimlendirme kuralı tarafından belirtilen veri çubuklarının ekseninin konumunu alır veya ayarlar. |
| [BarBorder](../../aspose.cells/databar/barborder) { get; } | Bir veri çubuğunun kenarlığını belirten bir nesne alır. |
| [BarFillType](../../aspose.cells/databar/barfilltype) { get; set; } | Bir veri çubuğunun renkle nasıl doldurulacağını alır veya ayarlar. |
| [Color](../../aspose.cells/databar/color) { get; set; } | Bu DataBar'ın Rengini alın veya ayarlayın. |
| [Direction](../../aspose.cells/databar/direction) { get; set; } | Veri çubuğunun görüntülendiği yönü alır veya ayarlar. |
| [MaxCfvo](../../aspose.cells/databar/maxcfvo) { get; } | Bu DataBar'ın maksimum değer nesnesini alın veya ayarlayın. FormatConditionValueType.Min türüyle null veya CFValueObject ayarlanamıyor. |
| [MaxLength](../../aspose.cells/databar/maxlength) { get; set; } | Veri çubuğunun maksimum uzunluğunu temsil eder. |
| [MinCfvo](../../aspose.cells/databar/mincfvo) { get; } | Bu DataBar'ın minimum değer nesnesini alın veya ayarlayın. FormatConditionValueType.Max türüyle null veya CFValueObject ayarlanamıyor. |
| [MinLength](../../aspose.cells/databar/minlength) { get; set; } | Veri çubuğunun minimum uzunluğunu temsil eder. |
| [NegativeBarFormat](../../aspose.cells/databar/negativebarformat) { get; } | Bir veri çubuğu koşullu biçimlendirme kuralıyla ilişkili NegativeBarFormat nesnesini alır. |
| [ShowValue](../../aspose.cells/databar/showvalue) { get; set; } | Bu veri çubuğunun uygulandığı hücrelerin değerlerinin gösterilip gösterilmeyeceğini belirten bayrağı alın veya ayarlayın. Varsayılan değer true. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [ToImage](../../aspose.cells/databar/toimage)(Cell, ImageOrPrintOptions) | Hücredeki veri çubuğunu görüntü bayt dizisine dönüştürün. |

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

ca.EndRow = 2;

ca.StartColumn = 0;

ca.EndColumn = 0;

fcs.AddArea(ca);

//Koşul ekler.
int idx = fcs.AddCondition(FormatConditionType.DataBar);

fcs.AddArea(ca);

FormatCondition cond = fcs[idx];

// Veri Çubuğunu Al
DataBar dataBar = cond.DataBar;

dataBar.Color = Color.Orange;

// Veri Çubuğu özelliklerini ayarla
dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;

dataBar.MinCfvo.Value = 30;

dataBar.ShowValue = false;

dataBar.BarBorder.Type = DataBarBorderType.Solid;

dataBar.BarBorder.Color = Color.Plum;

 dataBar.BarFillType = DataBarFillType.Solid;
  
 dataBar.AxisColor = Color.Red;
 
 dataBar.AxisPosition = DataBarAxisPosition.Midpoint;
 
 dataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
 
 dataBar.NegativeBarFormat.Color = Color.White;
 
 dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
 
 dataBar.NegativeBarFormat.BorderColor = Color.Yellow;
 
//Hücre Değerlerini Koy
Aspose.Cells.Cell cell1 = sheet.Cells["A1"];

cell1.PutValue(10);

Aspose.Cells.Cell cell2 = sheet.Cells["A2"];

cell2.PutValue(120);

Aspose.Cells.Cell cell3 = sheet.Cells["A3"];

cell3.PutValue(260);

//Excel dosyasını kaydetme
workbook.Save("book1.xlsx");

[VB.NET]

'Bir Çalışma Kitabı nesnesini başlatma
Dim workbook As Workbook = New Workbook()

Dim sheet As Worksheet = workbook.Worksheets(0)

'Boş bir koşullu biçimlendirme ekler
Dim index As Integer = sheet.ConditionalFormattings.Add()

Dim fcs As FormatConditionCollection = sheet.ConditionalFormattings(index)

'Koşullu biçim aralığını ayarlar.
Dim ca As New CellArea()

ca.StartRow = 0

ca.EndRow = 2

ca.StartColumn = 0

ca.EndColumn = 0

fcs.AddArea(ca)

'Koşul ekler.
Dim idx As Integer = fcs.AddCondition(FormatConditionType.DataBar)

fcs.AddArea(ca)

Dim cond As FormatCondition = fcs(idx)

'Veri Çubuğunu Alın
Dim dataBar As DataBar = cond.DataBar

dataBar.Color = Color.Orange

'Veri Çubuğu özelliklerini ayarla
dataBar.MinCfvo.Type = FormatConditionValueType.Percentile

dataBar.MinCfvo.Value = 30

dataBar.ShowValue = False

dataBar.BarBorder.Type = DataBarBorderType.Solid

dataBar.BarBorder.Color = Color.Plum

 dataBar.BarFillType = DataBarFillType.Solid
  
 dataBar.AxisColor = Color.Red
 
 dataBar.AxisPosition = DataBarAxisPosition.Midpoint
 
 dataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color
 
 dataBar.NegativeBarFormat.Color = Color.White
 
 dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color
 
 dataBar.NegativeBarFormat.BorderColor = Color.Yellow

'Hücre Değerlerini Koy
Dim cell1 As Aspose.Cells.Cell = sheet.Cells("A1")

cell1.PutValue(10)

Dim cell2 As Aspose.Cells.Cell = sheet.Cells("A2")

cell2.PutValue(120)

Dim cell3 As Aspose.Cells.Cell = sheet.Cells("A3")

cell3.PutValue(260)

'Excel dosyasını kaydetme
workbook.Save("book1.xlsx")

```

### Ayrıca bakınız

* ad alanı [Aspose.Cells](../../aspose.cells)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
