---
title: ExternalLinkCollection
second_title: Aspose.Cells för .NET API-referens
description: Representerar extern länksamling i en arbetsbok.
type: docs
weight: 3370
url: /sv/net/aspose.cells/externallinkcollection/
---
## ExternalLinkCollection class

Representerar extern länksamling i en arbetsbok.

```csharp
public class ExternalLinkCollection : IEnumerable
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Count](../../aspose.cells/externallinkcollection/count) { get; } | Hämtar antalet element som faktiskt finns i samlingen. |
| [Item](../../aspose.cells/externallinkcollection/item) { get; } | Får[`ExternalLink`](../externallink) element vid angivet index. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells/externallinkcollection/add#add_1)(string, string[]) | Lägger till en extern länk. |
| [Add](../../aspose.cells/externallinkcollection/add#add)(DirectoryType, string, string[]) | Lägg till en extern länk . |
| [Clear](../../aspose.cells/externallinkcollection/clear#clear)() | Tar bort alla externa länkar. |
| [Clear](../../aspose.cells/externallinkcollection/clear#clear_1)(bool) | Tar bort alla externa länkar. |
| [GetEnumerator](../../aspose.cells/externallinkcollection/getenumerator)() | Skaffa en uppräkning som itererar genom den här samlingen. |
| [RemoveAt](../../aspose.cells/externallinkcollection/removeat#removeat)(int) | Tar bort den angivna externa länken från arbetsboken. |
| [RemoveAt](../../aspose.cells/externallinkcollection/removeat#removeat_1)(int, bool) | Tar bort den angivna externa länken från arbetsboken. |

### Exempel

```csharp
[C#]
//Öppna en fil med externa länkar
Workbook workbook = new Workbook("book1.xls");

//Ändra extern länkdatakälla
workbook.Worksheets.ExternalLinks[0].DataSource = "d:\\link.xls";


[Visual Basic]
'Öppna en fil med externa länkar
Dim workbook As Workbook =  New Workbook("book1.xls")

'Ändra extern länkdatakälla
workbook.Worksheets.ExternalLinks(0).DataSource = "d:\\link.xls"
```

### Se även

* namnutrymme [Aspose.Cells](../../aspose.cells)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->