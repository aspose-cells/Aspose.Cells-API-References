---
title: "Sınıf Adı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Name sınıfı. Hücre aralığı için tanımlı bir adı temsil eder."
type: docs
url: /tr/net/aspose.cells/name/
---
## Name class

Hücre aralığı için tanımlanmış bir adı temsil eder.

```csharp
public class Name
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Comment](../../aspose.cells/name/comment/) { get; set; } | Adın yorumunu alır ve ayarlar. Yalnızca Excel 2007 veya daha yeni sürümler için geçerlidir. |
| [FullText](../../aspose.cells/name/fulltext/) { get; } | Kapsam ayarıyla nesnenin tam ad metnini alır. |
| [IsReferred](../../aspose.cells/name/isreferred/) { get; } | Bu adın diğer formüller tarafından referans alınıp alınmadığını gösterir. |
| [IsVisible](../../aspose.cells/name/isvisible/) { get; set; } | Adın görünür olup olmadığını gösterir. |
| [R1C1RefersTo](../../aspose.cells/name/r1c1refersto/) { get; set; } | `Name`'in bir R1C1 referansını alır veya ayarlar. |
| [RefersTo](../../aspose.cells/name/refersto/) { get; set; } | Adın referans vermek üzere tanımlandığı formülü, eşittir işaretiyle başlayan, alır veya ayarlar. |
| [SheetIndex](../../aspose.cells/name/sheetindex/) { get; set; } | Bu adın Workbook'a mı yoksa Worksheet'e mi ait olduğunu gösterir. 0 = Küresel ad, aksi takdirde sayfa indeksi (bir tabanlı). |
| [Text](../../aspose.cells/name/text/) { get; set; } | Nesnenin ad metnini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [GetRange](../../aspose.cells/name/getrange/#getrange)() | Bu ad bir aralığa referans veriyorsa aralığı alır. |
| [GetRange](../../aspose.cells/name/getrange/#getrange_1)(bool) | Bu ad bir aralığa referans veriyorsa aralığı alır |
| [GetRange](../../aspose.cells/name/getrange/#getrange_2)(int, int, int) | Bu ad bir aralığa referans veriyorsa aralığı alır. Eğer bu adın referansı mutlak değilse, aralık farklı hücreler için değişebilir. |
| [GetRanges](../../aspose.cells/name/getranges/#getranges)() | Bu ad tarafından referans verilen tüm aralıkları alır. |
| [GetRanges](../../aspose.cells/name/getranges/#getranges_1)(bool) | Bu ad tarafından referans verilen tüm aralıkları alır. |
| [GetReferredAreas](../../aspose.cells/name/getreferredareas/)(bool) | Bu ad tarafından referans verilen tüm referansları alır. |
| [GetRefersTo](../../aspose.cells/name/getrefersto/#getrefersto)(bool, bool) | Bu Name'in referansını al. |
| [GetRefersTo](../../aspose.cells/name/getrefersto/#getrefersto_1)(bool, bool, int, int) | Belirtilen hücreye göre bu Name'in referansını al. |
| [SetRefersTo](../../aspose.cells/name/setrefersto/)(string, bool, bool) | Bu Name'in referansını ayarla. |
| override [ToString](../../aspose.cells/name/tostring/)() | Geçerli Range nesnesini temsil eden bir dize döndürür. |

### Örnekler

```csharp

[C#]

//Workbook nesnesi örnekleniyor
Workbook workbook = new Workbook();
//Excel dosyasındaki ilk çalışma sayfasına erişim
Worksheet worksheet = workbook.Worksheets[0];
//Adlandırılmış bir aralık oluşturma
Range range = worksheet.Cells.CreateRange("B4", "G14");
//Adlandırılmış aralığın adını ayarlama
range.Name = "TestRange";
//Değiştirilmiş Excel dosyasını varsayılan (yani Excel 2000) formatta kaydetme
workbook.Save("output.xls");   

[Visual Basic]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()
'Accessing the first worksheet in the Excel file
Dim worksheet As Worksheet = workbook.Worksheets(0)
'Creating a named range
Dim range As Range = worksheet.Cells.CreateRange("B4", "G14")
'Setting the name of the named range
range.Name = "TestRange"
'Saving the modified Excel file in default (that is Excel 2000) format
workbook.Save("output.xls")
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


