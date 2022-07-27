---
title: ConditionalFormattingCollection
second_title: Aspose.Cells for .NET API Referansı
description: Bir koleksiyonu kapsüllerFormatCondition./formatcondition nesneler.
type: docs
weight: 1100
url: /tr/net/aspose.cells/conditionalformattingcollection/
---
## ConditionalFormattingCollection class

Bir koleksiyonu kapsüller[`FormatCondition`](../formatcondition) nesneler.

```csharp
public class ConditionalFormattingCollection : CollectionBase<FormatConditionCollection>
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells/conditionalformattingcollection/item) { get; } | Belirtilen dizindeki FormatConditions öğesini alır. |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [Add](../../aspose.cells/conditionalformattingcollection/add)() | Koleksiyona bir FormatConditions ekler. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(FormatConditionCollection) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(FormatConditionCollection, IComparer&lt;FormatConditionCollection&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, FormatConditionCollection, IComparer&lt;FormatConditionCollection&gt;) |  |
| [Clear](../../aspose.cells/collectionbase`1/clear)() |  |
| [Contains](../../aspose.cells/collectionbase`1/contains)(FormatConditionCollection) |  |
| [Copy](../../aspose.cells/conditionalformattingcollection/copy)(ConditionalFormattingCollection) | Koşullu biçimlendirmeyi kopyalar. |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(FormatConditionCollection[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(FormatConditionCollection[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, FormatConditionCollection[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;FormatConditionCollection&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(FormatConditionCollection) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(FormatConditionCollection, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(FormatConditionCollection, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(FormatConditionCollection) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(FormatConditionCollection, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(FormatConditionCollection, int, int) |  |
| [RemoveArea](../../aspose.cells/conditionalformattingcollection/removearea)(int, int, int, int) | Aralıktaki tüm koşullu biçimlendirmeyi kaldırın. |
| [RemoveAt](../../aspose.cells/collectionbase`1/removeat)(int) |  |

### Örnekler

```csharp

[C#]

//Bir Çalışma Kitabı nesnesini başlatma
Workbook workbook = new Workbook();

Worksheet sheet = workbook.Worksheets[0];

//Koşullu Biçimlendirmeyi Al
ConditionalFormattingCollection cformattings = sheet.ConditionalFormattings;

//Boş bir koşullu biçimlendirme ekler
int index = cformattings.Add();

//Yeni eklenen Koşullu biçimlendirmeyi al
FormatConditionCollection fcs = cformattings[index];

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

//Koşul ekle.
int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");

//Koşul ekle.
int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");

//Arka plan rengini ayarlar.
FormatCondition fc = fcs[conditionIndex];

fc.Style.BackgroundColor = Color.Red;

//Excel dosyasını kaydetme
workbook.Save("output.xls");

[VB.NET]

'Bir Çalışma Kitabı nesnesini başlatma
DDim workbook As Workbook = New Workbook()

Dim sheet As Worksheet = workbook.Worksheets(0)

'Koşullu Biçimlendirmeyi Alın
Dim cformattings As ConditionalFormattingCollection = sheet.ConditionalFormattings

'Boş bir koşullu biçimlendirme ekler
Dim index As Integer = cformattings.Add()

'Yeni eklenen Koşullu biçimlendirmeyi alın
Dim fcs As FormatConditionCollection = cformattings(index)

'Koşullu biçim aralığını ayarlar.
Dim ca As New CellArea()

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

'Koşul ekleyin.
Dim conditionIndex As Integer = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100")

'Koşul ekleyin.
Dim conditionIndex2 As Integer = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100")

'Arka plan rengini ayarlar.
Dim fc As FormatCondition = fcs(conditionIndex)

fc.Style.BackgroundColor = Color.Red

'Excel dosyasını kaydetme
workbook.Save("output.xls")
```

### Ayrıca bakınız

* class [CollectionBase&lt;T&gt;](../collectionbase-1)
* class [FormatConditionCollection](../formatconditioncollection)
* ad alanı [Aspose.Cells](../../aspose.cells)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
