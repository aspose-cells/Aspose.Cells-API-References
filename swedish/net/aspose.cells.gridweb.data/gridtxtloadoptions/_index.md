---
title: "Klass GridTxtLoadOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridWeb.Data.GridTxtLoadOptions-klass. Representerar alternativen för att läsa in textfil"
type: docs
url: /sv/net/aspose.cells.gridweb.data/gridtxtloadoptions/
---
## GridTxtLoadOptions class

Representerar alternativen för att läsa in en textfil.

```csharp
[Obsolete("This class will be obsoleted after stand alone dll usage of cells public api,instead you can use Aspose.Cells.TxtLoadOptions ")]
public class GridTxtLoadOptions : GridLoadOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [GridTxtLoadOptions](gridtxtloadoptions/)() | Skapar alternativen för att läsa in textfil. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AutoFilter](../../aspose.cells.gridweb.data/gridloadoptions/autofilter/) { get; set; } | Anger om data automatiskt filtreras vid inläsning av filerna.(Ärvd från [`GridLoadOptions`](../gridloadoptions/).) |
| [CheckDataValid](../../aspose.cells.gridweb.data/gridloadoptions/checkdatavalid/) { get; set; } | Kontrollera om data är giltiga i mallfilen.(Ärvd från [`GridLoadOptions`](../gridloadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells.gridweb.data/gridloadoptions/checkexcelrestriction/) { get; set; } | Om restriktioner för Excel-filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att mata in en strängvärde längre än 32K. När du matar in ett värde längre än 32K, t.ex. med Cell.PutValue(string), får du ett undantag om denna egenskap är sann. Om egenskapen är falsk accepterar vi ditt inmatade strängvärde som cellens värde så att du senare kan skriva ut hela strängvärdet för andra filformat som CSV. Däremot, om du har angett ett sådant värde som är ogiltigt för Excel-filformatet, bör du inte spara arbetsboken som Excel-filformat senare. Annars kan det uppstå oväntade fel i den genererade Excel-filen.(Ärvd från [`GridLoadOptions`](../gridloadoptions/).) |
| [ConvertDateTimeData](../../aspose.cells.gridweb.data/gridtxtloadoptions/convertdatetimedata/) { get; set; } | Hämtar eller anger ett värde som anger om strängen i textfilen konverteras till datumdata. |
| [ConvertNumericData](../../aspose.cells.gridweb.data/gridtxtloadoptions/convertnumericdata/) { get; set; } | Hämtar eller anger ett värde som anger om strängen i textfilen konverteras till numerisk data. |
| [Encoding](../../aspose.cells.gridweb.data/gridtxtloadoptions/encoding/) { get; set; } | Hämtar och anger standardkodningen. Gäller endast för csv-fil. |
| [ExtendToNextSheet](../../aspose.cells.gridweb.data/gridtxtloadoptions/extendtonextsheet/) { get; set; } | Om data ska utökas till nästa blad när rader eller kolumner överskrider gränsen. Om denna egenskap är sann, kommer extra data att utökas till nästa blad bakom det aktuella (om det aktuella bladet är det sista, kommer ett nytt blad att läggas till i den aktuella arbetsboken). Om egenskapen är falsk, kommer data som överskrider gränsen att ignoreras. Standardvärdet är falskt; |
| [HasFormula](../../aspose.cells.gridweb.data/gridtxtloadoptions/hasformula/) { get; set; } | Anger om texten är en formel om den börjar med "=". |
| [HasTextQualifier](../../aspose.cells.gridweb.data/gridtxtloadoptions/hastextqualifier/) { get; set; } | Om det finns textavgränsare för cellvärde. Standard är sant. |
| [IgnoreNotPrinted](../../aspose.cells.gridweb.data/gridloadoptions/ignorenotprinted/) { get; set; } | Ignorera data som inte skrivs ut om filen skrivs ut direkt(Ärvd från [`GridLoadOptions`](../gridloadoptions/).) |
| [IsMultiEncoded](../../aspose.cells.gridweb.data/gridtxtloadoptions/ismultiencoded/) { get; set; } | Sant betyder att filen innehåller flera kodningar. |
| [KeepPrecision](../../aspose.cells.gridweb.data/gridtxtloadoptions/keepprecision/) { get; set; } | Indikerar om en strängvärde inte ska parsas om längden är 15. |
| [KeepUnparsedData](../../aspose.cells.gridweb.data/gridloadoptions/keepunparseddata/) { get; set; } | Om de oparserade data ska hållas i minnet för arbetsboken när den läses in från mallfilen. Standard är sant.(Ärvd från [`GridLoadOptions`](../gridloadoptions/).) |
| [OnlyAuto](../../aspose.cells.gridweb.data/gridloadoptions/onlyauto/) { get; set; } | Anger om endast rader vars höjd inte är anpassad ska anpassas.(Ärvd från [`GridLoadOptions`](../gridloadoptions/).) |
| [ParsingFormulaOnOpen](../../aspose.cells.gridweb.data/gridloadoptions/parsingformulaonopen/) { get; set; } | Anger om formeln ska parsas när filen läses.(Ärvd från [`GridLoadOptions`](../gridloadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells.gridweb.data/gridloadoptions/parsingpivotcachedrecords/) { get; set; } | Anger om pivot-cachade poster ska parsas vid inläsning av filen. Standardvärdet är falskt.(Ärvd från [`GridLoadOptions`](../gridloadoptions/).) |
| [Password](../../aspose.cells.gridweb.data/gridloadoptions/password/) { get; set; } | Hämtar och anger lösenordet för arbetsboken.(Ärvd från [`GridLoadOptions`](../gridloadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells.gridweb.data/gridloadoptions/preservepaddingspacesinformula/) { get; set; } | Anger om mellanslag och radbrytningar som är insatta mellan formeltoken ska bevaras vid hämtning och inställning av formler. Standardvärdet är falskt.(Ärvd från [`GridLoadOptions`](../gridloadoptions/).) |
| [Separator](../../aspose.cells.gridweb.data/gridtxtloadoptions/separator/) { get; set; } | Hämtar och anger teckenseparator för textfil. |
| [SeparatorString](../../aspose.cells.gridweb.data/gridtxtloadoptions/separatorstring/) { get; set; } | Hämtar och anger ett strängvärde som avgränsare. |
| [TextQualifier](../../aspose.cells.gridweb.data/gridtxtloadoptions/textqualifier/) { get; set; } | Anger textavgränsaren för cellvärden. Standardavgränsaren är '\"'. |
| [TreatConsecutiveDelimitersAsOne](../../aspose.cells.gridweb.data/gridtxtloadoptions/treatconsecutivedelimitersasone/) { get; set; } | Om på varandra följande avgränsare ska behandlas som en. |
| [TreatQuotePrefixAsValue](../../aspose.cells.gridweb.data/gridtxtloadoptions/treatquoteprefixasvalue/) { get; set; } | Anger om det inledande enkelfnuttstecknet ska tas med som en del av värdet i en cell. Standard är true. Om det är false kommer det inledande enkelfnuttstecknet att tas bort från motsvarande cells värde och [`QuotePrefix`](../../aspose.cells.gridweb/gridtableitemstyle/quoteprefix/) kommer att sättas till true för cellen. |

### Se även

* class [GridLoadOptions](../gridloadoptions/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


