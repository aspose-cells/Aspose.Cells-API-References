---
title: Top10
second_title: Aspose.Cells for .NET API Referansı
description: İlk 10 koşullu biçimlendirme kuralını açıklayın. Bu koşullu biçimlendirme kuralı belirtildiği gibi değerleri üst N veya alt N ayracına giren hücreleri vurgular.
type: docs
weight: 6090
url: /tr/net/aspose.cells/top10/
---
## Top10 class

İlk 10 koşullu biçimlendirme kuralını açıklayın. Bu koşullu biçimlendirme kuralı, belirtildiği gibi, değerleri üst N veya alt N ayracına giren hücreleri vurgular.

```csharp
public class Top10
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [Top10](top10)() | Default_Constructor |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [IsBottom](../../aspose.cells/top10/isbottom) { get; set; } | Bir "üst/alt n" kuralının "alt n" kuralı olup olmadığını alın veya ayarlayın. Varsayılan değer false'tur. |
| [IsPercent](../../aspose.cells/top10/ispercent) { get; set; } | Bir "üst/alt n" kuralının bir "üst/alt yüzde n" kuralı olup olmadığını alın veya ayarlayın. Varsayılan değer false'tur. |
| [Rank](../../aspose.cells/top10/rank) { get; set; } | Bir "üst/alt n" koşullu biçimlendirme kuralında "n" değerini alın veya ayarlayın. IsPercent değeri doğruysa, değer 0 ile 100 arasında olmalıdır. Aksi takdirde 0 ile 1000 arasında olmalıdır. Varsayılan değer 10'dur . |

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
CellArea ca = CellArea.CreateCellArea(0, 0, 10, 10);
fcs.AddArea(ca);
 
//Koşul ekler.
int conditionIndex = fcs.AddCondition(FormatConditionType.Top10, OperatorType.None, null, null);   
//Arka plan rengini ayarlar.
FormatCondition fc = fcs[conditionIndex];
fc.Style.BackgroundColor = Color.Red;
Top10 top10 = fc.Top10;
// İlk N'yi Ayarla 
top10.Rank = 5;  
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
Dim ca As CellArea = CellArea.CreateCellArea(0, 0, 10, 10)
fcs.AddArea(ca)
 
'Koşul ekler.
Dim conditionIndex As Integer = fcs.AddCondition(FormatConditionType.Top10, OperatorType.None, null, null);   
'Arka plan rengini ayarlar.
Dim fc As FormatCondition = fcs(conditionIndex)
fc.Style.BackgroundColor = Color.Red
Dim top10 as Top10  = fc.Top10
'İlk N'yi Ayarla 
top10.Rank = 5
'Excel dosyasını kaydetme
workbook.Save("output.xls")
```

### Ayrıca bakınız

* ad alanı [Aspose.Cells](../../aspose.cells)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
