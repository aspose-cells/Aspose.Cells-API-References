---
title: "Klass GridWorkbookSettings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridJs.GridWorkbookSettings‑klass. Representerar arbetsbokens inställningar"
type: docs
url: /sv/net/aspose.cells.gridjs/gridworkbooksettings/
---
## GridWorkbookSettings class

Representerar inställningarna för arbetsboken.

```csharp
public class GridWorkbookSettings
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [GridWorkbookSettings](gridworkbooksettings/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Author](../../aspose.cells.gridjs/gridworkbooksettings/author/) { get; set; } | Hämtar/Anger filens författare. |
| [CheckCustomNumberFormat](../../aspose.cells.gridjs/gridworkbooksettings/checkcustomnumberformat/) { get; set; } | Anger om anpassade talformat ska kontrolleras när Style.Custom sätts, standardvärdet är `false`. |
| [CheckExcelRestriction](../../aspose.cells.gridjs/gridworkbooksettings/checkexcelrestriction/) { get; set; } | Anger om begränsningar i Excel‑filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att mata in en strängvärde längre än 32 KB. När du matar in ett värde längre än 32 KB, t.ex. via Cell.PutValue(string), får du ett undantag om denna egenskap är `true`. Om egenskapen är `false` accepterar vi ditt inmatade strängvärde som cellens värde så att du senare kan exportera hela strängen till andra filformat som CSV. Dock, om du har angett ett värde som är ogiltigt för Excel‑filformatet bör du inte spara arbetsboken som Excel‑format senare. Annars kan det uppstå oväntade fel i den genererade Excel‑filen. Standardvärdet är `false`. |
| [CreateCalcChain](../../aspose.cells.gridjs/gridworkbooksettings/createcalcchain/) { get; set; } | Anger om en kedja av beräknade formler ska skapas. Standardvärdet är `false`. |
| [Date1904](../../aspose.cells.gridjs/gridworkbooksettings/date1904/) { get; set; } | Hämtar eller anger ett värde som visar om arbetsboken använder 1904-datersystemet. |
| [EnableMacros](../../aspose.cells.gridjs/gridworkbooksettings/enablemacros/) { get; set; } | Aktivera makron; Detta fungerar för närvarande endast när ett arbetsblad kopieras till ett annat arbetsblad i en arbetsbok. |
| [ForceFullCalculate](../../aspose.cells.gridjs/gridworkbooksettings/forcefullcalculate/) { get; set; } | Anger om hela beräkningen ska utföras varje gång en beräkning utlöses. |
| [Iteration](../../aspose.cells.gridjs/gridworkbooksettings/iteration/) { get; set; } | Anger om iteration ska användas för att lösa cirkulära referenser. |
| [MaxIteration](../../aspose.cells.gridjs/gridworkbooksettings/maxiteration/) { get; set; } | Returnerar eller anger det maximala antalet iterationer för att lösa en cirkulär referens, standardvärdet är 100. |
| [PrecisionAsDisplayed](../../aspose.cells.gridjs/gridworkbooksettings/precisionasdisplayed/) { get; set; } | Sant om beräkningarna i denna arbetsbok endast utförs med den precision som siffrorna visas med |
| [ReCalculateOnOpen](../../aspose.cells.gridjs/gridworkbooksettings/recalculateonopen/) { get; set; } | Anger om alla formler ska beräknas om vid öppning av filen. Standard är true. |

### Exempel

```csharp
[C#]

GridJsWorkbook g = new GridJsWorkbook();

GridWorkbookSettings gsettings = new GridWorkbookSettings();
g.Settings=gsettings;

//utför din verksamhet

[Visual Basic]
Dim g as GridJsWorkbook = new GridJsWorkbook()

Dim gsettings as GridWorkbookSettings = new GridWorkbookSettings()
 g.Settings=gsettings;
 
'do your business
```

### Se även

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


