---
title: ExternalLink
second_title: Aspose.Cells for .NET API Referansı
description: Çalışma kitabındaki harici bir bağlantıyı temsil eder.
type: docs
weight: 3360
url: /tr/net/aspose.cells/externallink/
---
## ExternalLink class

Çalışma kitabındaki harici bir bağlantıyı temsil eder.

```csharp
public class ExternalLink
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [DataSource](../../aspose.cells/externallink/datasource) { get; set; } | Harici bağlantının veri kaynağını temsil eder. |
| [IsReferred](../../aspose.cells/externallink/isreferred) { get; } | Bu harici bağlantıya başkaları tarafından başvuruda bulunulup bulunulmadığını gösterir. |
| [IsVisible](../../aspose.cells/externallink/isvisible) { get; } | Bu harici bağlantının MS Excel'de görünür olup olmadığını gösterir. |
| [OriginalDataSource](../../aspose.cells/externallink/originaldatasource) { get; set; } | Harici bağlantının depolanan veri kaynağını temsil eder. |
| [Type](../../aspose.cells/externallink/type) { get; } | Harici bağlantının türünü alır. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [AddExternalName](../../aspose.cells/externallink/addexternalname)(string, string) | Harici bir ad ekler. |

### Örnekler

```csharp

[C#]

//Harici bağlantılar içeren bir dosya aç
Workbook workbook = new Workbook("book1.xls");

//Harici Bağlantı Al 
ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];

//Harici Bağlantının Veri Kaynağını Değiştir
externalLink.DataSource = "d:\\link.xls";

[VB.NET]

'Harici bağlantılar içeren bir dosya açın
Dim workbook As New Workbook("book1.xls")

'Harici Bağlantı Alın 
Dim externalLink As ExternalLink = workbook.Worksheets.ExternalLinks(0)

'Change External Link's Data Source
externalLink.DataSource = "d:\link.xls"
```

### Ayrıca bakınız

* ad alanı [Aspose.Cells](../../aspose.cells)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
