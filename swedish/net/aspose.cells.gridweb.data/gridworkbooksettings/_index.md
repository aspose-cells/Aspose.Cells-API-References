---
title: "Klass GridWorkbookSettings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridWeb.Data.GridWorkbookSettings‑klass. Representerar inställningarna för arbetsboken"
type: docs
url: /sv/net/aspose.cells.gridweb.data/gridworkbooksettings/
---
## GridWorkbookSettings class

Representerar inställningarna för arbetsboken.

```csharp
public class GridWorkbookSettings : ISerializable
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [GridWorkbookSettings](gridworkbooksettings/)() | standardkonstruktor |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Author](../../aspose.cells.gridweb.data/gridworkbooksettings/author/) { get; set; } | Hämtar och anger författaren till filen. |
| [CheckCustomNumberFormat](../../aspose.cells.gridweb.data/gridworkbooksettings/checkcustomnumberformat/) { get; set; } | Hämtar eller anger om anpassat talformat ska kontrolleras när Style.Custom sätts. |
| [CreateCalcChain](../../aspose.cells.gridweb.data/gridworkbooksettings/createcalcchain/) { get; set; } | Hämtar eller anger om en kedja av beräknade formler ska skapas. Standard är falskt. |
| [Date1904](../../aspose.cells.gridweb.data/gridworkbooksettings/date1904/) { get; set; } | Hämtar eller anger värdet som representerar om arbetsboken använder 1904-datumsystemet. |
| [EnableMacros](../../aspose.cells.gridweb.data/gridworkbooksettings/enablemacros/) { get; set; } | Hämtar eller anger om makron ska aktiveras; Nu fungerar det endast när ett kalkylblad kopieras till ett annat kalkylblad i en arbetsbok. |
| [ForceFullCalculate](../../aspose.cells.gridweb.data/gridworkbooksettings/forcefullcalculate/) { get; set; } | Hämtar eller anger om hela beräkningen ska utföras varje gång en beräkning utlöses. |
| [Iteration](../../aspose.cells.gridweb.data/gridworkbooksettings/iteration/) { get; set; } | Hämtar eller anger om iteration ska användas för att lösa cirkulära referenser. |
| [MaxIteration](../../aspose.cells.gridweb.data/gridworkbooksettings/maxiteration/) { get; set; } | Hämtar eller anger det maximala antalet iterationer för att lösa en cirkulär referens, standardvärdet är 100. |
| [PrecisionAsDisplayed](../../aspose.cells.gridweb.data/gridworkbooksettings/precisionasdisplayed/) { get; set; } | Sant om beräkningarna i denna arbetsbok endast utförs med den precision som siffrorna visas med |
| [PreservePaddingSpaces](../../aspose.cells.gridweb.data/gridworkbooksettings/preservepaddingspaces/) { get; set; } | Anger om mellanslag och radbrytningar som finns mellan formeltoken ska bevaras vid hämtning och angivning av formler. Standardvärdet är false. |
| [ReCalculateOnOpen](../../aspose.cells.gridweb.data/gridworkbooksettings/recalculateonopen/) { get; set; } | Hämtar eller anger om alla formler ska beräknas om vid öppning av filen. |

### Exempel

```csharp
[C#]

 
GridWeb gridweb = new GridWeb();
GridWorkbookSettings gsettings = new GridWorkbookSettings();
gridweb.Settings=gsettings;

//utför din verksamhet

[Visual Basic]


Dim gsettings as GridWorkbookSettings = new GridWorkbookSettings()
 gridweb.Settings=gsettings;
 
'do your business
```

### Se även

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


