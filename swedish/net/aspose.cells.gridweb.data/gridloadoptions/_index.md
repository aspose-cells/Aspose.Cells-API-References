---
title: "Klass GridLoadOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridWeb.Data.GridLoadOptions-klass. Representerar alternativ för att ladda filen. Föråldrad. Den här klassen kommer att föråldras efter fristående dll-användning av cells offentliga API, istället kan du använda Aspose.Cells.LodOptions"
type: docs
url: /sv/net/aspose.cells.gridweb.data/gridloadoptions/
---
## GridLoadOptions class

Representerar alternativ för att ladda filen. [Obsolete(\"Denna klass kommer att föråldras efter fristående dll-användning av cells offentliga api, använd istället Aspose.Cells.LodOptions \")]

```csharp
public class GridLoadOptions : ISerializable
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [GridLoadOptions](gridloadoptions/)() | Skapar alternativ för att läsa in filen. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AutoFilter](../../aspose.cells.gridweb.data/gridloadoptions/autofilter/) { get; set; } | Indikerar om data automatiskt filtreras vid inläsning av filerna. |
| [CheckDataValid](../../aspose.cells.gridweb.data/gridloadoptions/checkdatavalid/) { get; set; } | Kontrollera om data är giltiga i mallfilen. |
| [CheckExcelRestriction](../../aspose.cells.gridweb.data/gridloadoptions/checkexcelrestriction/) { get; set; } | Om restriktioner för Excel-filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att en strängvärde längre än 32 K matas in. När du matar in ett värde längre än 32 K, t.ex. med Cell.PutValue(string), får du ett undantag om den här egenskapen är sann. Om egenskapen är falsk accepterar vi ditt inmatade strängvärde som cellens värde så att du senare kan exportera hela strängvärdet till andra filformat som CSV. Däremot, om du har angett ett värde som är ogiltigt för Excel-filformatet bör du inte spara arbetsboken som Excel-filformat senare. Annars kan det uppstå oväntade fel i den genererade Excel-filen. |
| [IgnoreNotPrinted](../../aspose.cells.gridweb.data/gridloadoptions/ignorenotprinted/) { get; set; } | Ignorera data som inte skrivs ut om filen skrivs ut direkt. |
| [KeepUnparsedData](../../aspose.cells.gridweb.data/gridloadoptions/keepunparseddata/) { get; set; } | Om de oparsade data ska behållas i minnet för Workbook när den laddas från mallfilen. Standard är true. |
| [OnlyAuto](../../aspose.cells.gridweb.data/gridloadoptions/onlyauto/) { get; set; } | Anger om endast rader vars höjd inte är anpassad ska anpassas. |
| [ParsingFormulaOnOpen](../../aspose.cells.gridweb.data/gridloadoptions/parsingformulaonopen/) { get; set; } | Anger om formeln ska parsas när filen läses. |
| [ParsingPivotCachedRecords](../../aspose.cells.gridweb.data/gridloadoptions/parsingpivotcachedrecords/) { get; set; } | Anger om pivot‑cachade poster ska parsas vid inläsning av filen. Standardvärdet är false. |
| [Password](../../aspose.cells.gridweb.data/gridloadoptions/password/) { get; set; } | Hämtar och anger lösenordet för Workbook. |
| [PreservePaddingSpacesInFormula](../../aspose.cells.gridweb.data/gridloadoptions/preservepaddingspacesinformula/) { get; set; } | Anger om mellanslag och radbrytningar som finns mellan formeltoken ska bevaras vid hämtning och angivning av formler. Standardvärdet är false. |

### Se även

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


