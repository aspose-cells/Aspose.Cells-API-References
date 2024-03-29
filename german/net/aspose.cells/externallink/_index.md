---
title: ExternalLink
second_title: Aspose.Cells für .NET-API-Referenz
description: Stellt einen externen Link in einer Arbeitsmappe dar.
type: docs
weight: 3360
url: /de/net/aspose.cells/externallink/
---
## ExternalLink class

Stellt einen externen Link in einer Arbeitsmappe dar.

```csharp
public class ExternalLink
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [DataSource](../../aspose.cells/externallink/datasource) { get; set; } | Stellt die Datenquelle des externen Links dar. |
| [IsReferred](../../aspose.cells/externallink/isreferred) { get; } | Gibt an, ob auf diesen externen Link von anderen verwiesen wird. |
| [IsVisible](../../aspose.cells/externallink/isvisible) { get; } | Gibt an, ob dieser externe Link in MS Excel sichtbar ist. |
| [OriginalDataSource](../../aspose.cells/externallink/originaldatasource) { get; set; } | Repräsentiert gespeicherte Datenquelle des externen Links. |
| [Type](../../aspose.cells/externallink/type) { get; } | Ruft den Typ des externen Links ab. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AddExternalName](../../aspose.cells/externallink/addexternalname)(string, string) | Fügt einen externen Namen hinzu. |

### Beispiele

```csharp

[C#]

//Öffne eine Datei mit externen Links
Workbook workbook = new Workbook("book1.xls");

//Externen Link abrufen 
ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];

//Datenquelle des externen Links ändern
externalLink.DataSource = "d:\\link.xls";

[VB.NET]

'Öffnen Sie eine Datei mit externen Links
Dim workbook As New Workbook("book1.xls")

'Holen Sie sich einen externen Link 
Dim externalLink As ExternalLink = workbook.Worksheets.ExternalLinks(0)

'Change External Link's Data Source
externalLink.DataSource = "d:\link.xls"
```

### Siehe auch

* namensraum [Aspose.Cells](../../aspose.cells)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
