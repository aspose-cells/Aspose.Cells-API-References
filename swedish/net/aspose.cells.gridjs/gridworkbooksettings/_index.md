---
title: GridWorkbookSettings
second_title: Aspose.Cells för .NET API-referens
description: Representerar inställningarna för arbetsboken.
type: docs
weight: 110
url: /sv/net/aspose.cells.gridjs/gridworkbooksettings/
---
## GridWorkbookSettings class

Representerar inställningarna för arbetsboken.

```csharp
public class GridWorkbookSettings
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [GridWorkbookSettings](gridworkbooksettings)() | Default_Constructor |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Author](../../aspose.cells.gridjs/gridworkbooksettings/author) { get; set; } | Hämtar och ställer in författaren till filen. |
| [CheckCustomNumberFormat](../../aspose.cells.gridjs/gridworkbooksettings/checkcustomnumberformat) { get; set; } | Indikerar om anpassat talformat kontrolleras vid inställning av Style.Custom. |
| [CreateCalcChain](../../aspose.cells.gridjs/gridworkbooksettings/createcalcchain) { get; set; } | Indikerar om du skapar beräknade formlerkedja. Standard är false. |
| [Date1904](../../aspose.cells.gridjs/gridworkbooksettings/date1904) { get; set; } | Hämtar eller ställer in ett värde som representerar om arbetsboken använder 1904-datumsystemet. |
| [EnableMacros](../../aspose.cells.gridjs/gridworkbooksettings/enablemacros) { get; set; } | Aktivera makron; Nu fungerar det bara när du kopierar ett kalkylblad till ett annat kalkylblad i en arbetsbok. |
| [ForceFullCalculate](../../aspose.cells.gridjs/gridworkbooksettings/forcefullcalculate) { get; set; } | Indikerar om fullständigt beräknas varje gång när en beräkning utlöses. |
| [Iteration](../../aspose.cells.gridjs/gridworkbooksettings/iteration) { get; set; } | Indikerar om använd iteration för att lösa cirkulära referenser. |
| [MaxIteration](../../aspose.cells.gridjs/gridworkbooksettings/maxiteration) { get; set; } | Returnerar eller ställer in det maximala antalet iterationer för att lösa en cirkulär referens, standardvärdet är 100. |
| [PrecisionAsDisplayed](../../aspose.cells.gridjs/gridworkbooksettings/precisionasdisplayed) { get; set; } | Sant om beräkningar i den här arbetsboken kommer att göras med enbart precisionen hos siffrorna som de visas |
| [ReCalculateOnOpen](../../aspose.cells.gridjs/gridworkbooksettings/recalculateonopen) { get; set; } | Indikerar om alla formler ska räknas om när filen öppnas. |

### Exempel

```csharp
[C#]

GridJsWorkbook g = new GridJsWorkbook();

GridWorkbookSettings gsettings = new GridWorkbookSettings();
g.Settings=gsettings;

//gör dina affärer

[Visual Basic]
Dim g as GridJsWorkbook = new GridJsWorkbook()

Dim gsettings as GridWorkbookSettings = new GridWorkbookSettings()
 g.Settings=gsettings;
 
'göra dina affärer
```

### Se även

* namnutrymme [Aspose.Cells.GridJs](../../aspose.cells.gridjs)
* hopsättning [Aspose.Cells.GridJs](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridJs.dll -->
