---
title: ColumnCollection
second_title: Aspose.Cells for .NET API Referansı
description: Koleksiyonubir çalışma sayfasındaki bağımsız sütunları ayarları temsil eden nesneler. Sütun nesnesi yalnızca sütun genişliği stiller .vb. gibi ayarları temsil eder. tüm sütun için nin karşılık gelen sütunda boş hücreveri olmaması veya olmaması gerçeğiyle hiçbir ilgisi yoktur. Ve bu koleksiyonun Countu yalnızca bu sütunda somutlaştırılan count Column nesnelerini temsil eder. collection nin çalışma sayfasında boş olmayan hücrelerveri olup olmamasıyla hiçbir ilgisi yoktur.
type: docs
weight: 1070
url: /tr/net/aspose.cells/columncollection/
---
## ColumnCollection class

Koleksiyonubir çalışma sayfasındaki bağımsız sütunları (ayarları) temsil eden nesneler. Sütun nesnesi yalnızca sütun genişliği, stiller, .vb. gibi ayarları temsil eder. tüm sütun için, 'nin, karşılık gelen sütunda boş hücre(veri) olmaması veya olmaması gerçeğiyle hiçbir ilgisi yoktur. Ve bu koleksiyonun "Count"u, yalnızca bu sütunda somutlaştırılan count Column nesnelerini temsil eder. collection, 'nin çalışma sayfasında boş olmayan hücreler(veri) olup olmamasıyla hiçbir ilgisi yoktur.

```csharp
public class ColumnCollection : CollectionBase<Column>
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells/columncollection/item) { get; } | sütun indekse göre nesne. Verilen sütun dizininin Column nesnesi, daha önce mevcut değilse başlatılacaktır. |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Column) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Column, IComparer&lt;Column&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Column, IComparer&lt;Column&gt;) |  |
| [Clear](../../aspose.cells/collectionbase`1/clear)() |  |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Column) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Column[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Column[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Column[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;Column&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;Column&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;Column&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;Column&gt;) |  |
| [GetColumnByIndex](../../aspose.cells/columncollection/getcolumnbyindex)(int) | [`Column`](../column)listedeki konuma göre nesne. |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Column) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Column, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Column, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Column) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Column, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Column, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase`1/removeat)(int) |  |

### Örnekler

```csharp

[C#]

//Bir Çalışma Kitabı nesnesini başlatma
Workbook workbook = new Workbook();

//İlk çalışma sayfasının referansının alınması
Worksheet worksheet = workbook.Worksheets[0];

//Çalışma Kitabına yeni Stil ekle
Style style = workbook.CreateStyle();

//Arka plan rengini Mavi olarak ayarlama
style.ForegroundColor = Color.Blue;

// Arka Plan Desenini ayarlama
style.Pattern = BackgroundType.Solid;

//Yeni Stil Bayrağı
StyleFlag styleFlag = new StyleFlag();

// Tüm Stilleri Ayarla
styleFlag.All = true;

//İlk on sütunun varsayılan genişliğini değiştirin
for (int i = 0; i < 10; i++)
{
    worksheet.Cells.Columns[i].Width = 20;
}

// Varsayılan olmayan biçimlendirme ile Sütunu alın
ColumnCollection columns = worksheet.Cells.Columns;

foreach (Column column in columns)
{
    // Stili ilk on Sütuna uygula
    column.ApplyStyle(style, styleFlag);
}

//Excel dosyasını kaydetme
workbook.Save("book1.xls");

[VB.NET]

'Bir Çalışma Kitabı nesnesini başlatma
Dim workbook As Workbook = New Workbook()

'İlk çalışma sayfasının referansının alınması
Dim worksheet As Worksheet = workbook.Worksheets(0)

'Çalışma Kitabına Yeni Stil Ekle
Dim style As Style = workbook.CreateStyles()

'Arka plan rengini Mavi olarak ayarlama
style.ForegroundColor = Color.Blue

'Arka Plan Desenini ayarlama
style.Pattern = BackgroundType.Solid

'Yeni Stil Bayrağı
Dim styleFlag As New StyleFlag()

'Tüm Stilleri Ayarla
styleFlag.All = True

'İlk on sütunun varsayılan genişliğini değiştirin
For i As Integer = 0 To 9
    worksheet.Cells.Columns(i).Width = 20
Next i

'Varsayılan olmayan biçimlendirmeye sahip Sütunu alın
Dim columns As ColumnCollection = worksheet.Cells.Columns

For Each column As Column In columns
    'Stili ilk on Sütuna Uygula
    column.ApplyStyle(style, styleFlag)
Next column

'Excel dosyasını kaydetme
workbook.Save("book1.xls")

```

### Ayrıca bakınız

* class [CollectionBase&lt;T&gt;](../collectionbase-1)
* class [Column](../column)
* ad alanı [Aspose.Cells](../../aspose.cells)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
