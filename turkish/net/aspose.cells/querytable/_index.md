---
title: QueryTable
second_title: Aspose.Cells for .NET API Referansı
description: QueryTable bilgilerini temsil eder.
type: docs
weight: 4930
url: /tr/net/aspose.cells/querytable/
---
## QueryTable class

QueryTable bilgilerini temsil eder.

```csharp
public class QueryTable
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [AdjustColumnWidth](../../aspose.cells/querytable/adjustcolumnwidth) { get; set; } | Nesnenin AdjustColumnWidth değerini döndürür veya ayarlar. |
| [ConnectionId](../../aspose.cells/querytable/connectionid) { get; } | Sorgu tablosunun bağlantı kimliğini alır. |
| [ExternalConnection](../../aspose.cells/querytable/externalconnection) { get; } | İlgili harici bağlantıyı alır. |
| [Name](../../aspose.cells/querytable/name) { get; } | Sorgulanabilirin adını alır. |
| [PreserveFormatting](../../aspose.cells/querytable/preserveformatting) { get; set; } | Nesnenin PreserveFormatting değerini döndürür veya ayarlar. |
| [ResultRange](../../aspose.cells/querytable/resultrange) { get; } | Sonucun aralığını alır. |

### Örnekler

```csharp

[C#]

//Bir Çalışma Kitabı nesnesini başlatma
Workbook workbook = new Workbook();

//İlk çalışma sayfasının referansının alınması
Worksheet worksheet = workbook.Worksheets[0];
//Çalışma sayfasındaki ilk sorgu tablosunu alma
QueryTable qt = worksheet.QueryTables[0];
//Sorgu tablosunun görünen adresi alınıyor.
string address = qt.ResultRange.Address;

[VB.NET]

'Bir Çalışma Kitabı nesnesini başlatma
Dim workbook As Workbook = New Workbook()

'İlk çalışma sayfasının referansının alınması
Dim worksheet As Worksheet = workbook.Worksheets(0)
'Çalışma sayfasındaki ilk sorgu tablosunu alma
QueryTable qt = worksheet.QueryTables[0];
'Sorgu tablosunun görünen adresi alınıyor.
string address = qt.ResultRange.Address;
```

### Ayrıca bakınız

* ad alanı [Aspose.Cells](../../aspose.cells)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
