---
title: "Klass GridCell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridDesktop.Data.GridCell-klass. Representerar ett cellobjekt"
type: docs
url: /sv/net/aspose.cells.griddesktop.data/gridcell/
---
## GridCell class

Representerar ett cellobjekt.

```csharp
public class GridCell
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [BoolValue](../../aspose.cells.griddesktop.data/gridcell/boolvalue/) { get; } | Hämtar det booleska värdet som finns i cellen. |
| [Column](../../aspose.cells.griddesktop.data/gridcell/column/) { get; } | Hämtar kolumnnumret (nollbaserat) för cellen. |
| [DateValue](../../aspose.cells.griddesktop.data/gridcell/datevalue/) { get; } | Hämtar DateTime‑värdet som finns i cellen. |
| [DisplayStringValue](../../aspose.cells.griddesktop.data/gridcell/displaystringvalue/) { get; } | Hämtar det formaterade strängvärdet för den här cellen. |
| [DoubleValue](../../aspose.cells.griddesktop.data/gridcell/doublevalue/) { get; } | Hämtar dubbelvärdet som finns i cellen. |
| [FloatValue](../../aspose.cells.griddesktop.data/gridcell/floatvalue/) { get; } | Hämtar flyttalsvärdet som finns i cellen. |
| [Formula](../../aspose.cells.griddesktop.data/gridcell/formula/) { get; set; } | Hämtar eller anger en formel för cellen. |
| [HasCustomStyle](../../aspose.cells.griddesktop.data/gridcell/hascustomstyle/) { get; } | Anger om den här cellen har anpassade stilinställningar (annorlunda än standardinställningen som ärvs från motsvarande rad, kolumn eller arbetsbok). |
| [HtmlString](../../aspose.cells.griddesktop.data/gridcell/htmlstring/) { get; set; } | Hämtar och anger HTML-strängen som innehåller data och viss formatering i den här cellen. |
| [IntValue](../../aspose.cells.griddesktop.data/gridcell/intvalue/) { get; } | Hämtar heltalsvärdet som finns i cellen. |
| [IsStyleSet](../../aspose.cells.griddesktop.data/gridcell/isstyleset/) { get; } | Anger om cellens stil är angiven. Om den returnerar false betyder det att cellen har ett standardformat. |
| [Location](../../aspose.cells.griddesktop.data/gridcell/location/) { get; } |  |
| [Name](../../aspose.cells.griddesktop.data/gridcell/name/) { get; } | Hämtar namnet på cellen. Till exempel: A1, F102. |
| [Protected](../../aspose.cells.griddesktop.data/gridcell/protected/) { get; set; } | Anger om cellen är skyddad. Om värdet är "true" kan användaren inte ändra cellen via användargränssnittet. Detta attribut har ingen koppling till egenskapen Style.CellLocked och sparas inte till fil när rutnätsdata exporteras. Standardvärdet är "false". |
| [Row](../../aspose.cells.griddesktop.data/gridcell/row/) { get; } | Hämtar radnumret (nollbaserat) för cellen. |
| [StringValue](../../aspose.cells.griddesktop.data/gridcell/stringvalue/) { get; } | Hämtar strängvärdet som finns i cellen. |
| [Style](../../aspose.cells.griddesktop.data/gridcell/style/) { get; set; } | Hämtar en kopia av cellstilen. Ange stilen för cellen. |
| [Type](../../aspose.cells.griddesktop.data/gridcell/type/) { get; } | returnerar cellvärdestypen, betydelsen kan ses i GridCellValueType.java |
| [Value](../../aspose.cells.griddesktop.data/gridcell/value/) { get; set; } | Hämtar värdet som finns i den här cellen. |
| [Worksheet](../../aspose.cells.griddesktop.data/gridcell/worksheet/) { get; } | Hämtar kalkylbladsobjektet. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [ContainsExternalLink](../../aspose.cells.griddesktop.data/gridcell/containsexternallink/)() | Anger om den här cellen innehåller en extern länk. Gäller endast när cellen är en formelcell. |
| [Copy](../../aspose.cells.griddesktop.data/gridcell/copy/)(GridCell) | Kopierar data från en källcell. |
| [CopyStyle](../../aspose.cells.griddesktop.data/gridcell/copystyle/)(Style) | kopiera stilen och ange stilen för cellen |
| override [Equals](../../aspose.cells.griddesktop.data/gridcell/equals/)(object) |  |
| [GetCellArea](../../aspose.cells.griddesktop.data/gridcell/getcellarea/)() |  |
| [GetFont](../../aspose.cells.griddesktop.data/gridcell/getfont/)() | Hämtar cellens teckensnitt. När du ändrar teckensnittet bör du anropa metoden "SetFont" för att sätta teckensnittet i cellen. |
| [GetFontColor](../../aspose.cells.griddesktop.data/gridcell/getfontcolor/)() | Hämtar cellens teckensnittsfärg. När du ändrar färgen bör du anropa metoden "SetFontColor" för att sätta teckensnittsfärgen i cellen. |
| override [GetHashCode](../../aspose.cells.griddesktop.data/gridcell/gethashcode/)() |  |
| [GetStyle](../../aspose.cells.griddesktop.data/gridcell/getstyle/)() | Hämtar cellens stil. När du ändrar stilen bör du anropa metoden "SetStyle" för att sätta stilen i cellen. |
| [GetValidation](../../aspose.cells.griddesktop.data/gridcell/getvalidation/)() | Hämtar valideringen som tillämpas på den här cellen. Om den inte är angiven returneras null. |
| [GetWidthOfValue](../../aspose.cells.griddesktop.data/gridcell/getwidthofvalue/)() | Hämtar bredden på värdet i enheten pixlar. |
| [GetWorksheet](../../aspose.cells.griddesktop.data/gridcell/getworksheet/)() | Hämtar det överordnade kalkylbladet. |
| [IsErrorValue](../../aspose.cells.griddesktop.data/gridcell/iserrorvalue/)() | Kontrollerar om en formel kan utvärdera ett resultat korrekt. |
| [IsFormula](../../aspose.cells.griddesktop.data/gridcell/isformula/)() | Anger om den angivna cellen innehåller en formel. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue)(bool) | Sätter ett booleskt värde i cellen. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_3)(DateTime) | Sätter ett DateTime-värde i cellen. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_1)(double) | Sätter ett double-värde i cellen. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_2)(int) | Sätter ett heltalsvärde i cellen. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_4)(object) | Sätter ett objektvärde i cellen. Samma som setValue(Object param_object) |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_5)(string) | Sätter ett strängvärde i cellen. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_6)(string, bool) | Sätter ett strängvärde i cellen och konverterar värdet till annan datatyp om lämpligt. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_7)(string, bool, bool) | Sätter ett värde i cellen, om lämpligt kommer värdet att konverteras till annan datatyp och cellens talformat återställas. |
| [PutValueAndSetFormatByValue](../../aspose.cells.griddesktop.data/gridcell/putvalueandsetformatbyvalue/)(string) | Sätter cellens värde med ett strängvärde och anger cellformatet baserat på detta värde. |
| [SetCellValue](../../aspose.cells.griddesktop.data/gridcell/setcellvalue/)(object) | Om värdet är en formel, sätter denna metod cellens värde som FormulaType, |
| [SetCustom](../../aspose.cells.griddesktop.data/gridcell/setcustom/)(string) | sätter det anpassade formatet, null eller tom sträng betyder inget anpassat format. |
| [SetFont](../../aspose.cells.griddesktop.data/gridcell/setfont/)(Font) | Sätter teckensnittet i cellen. För att förbättra prestanda, implementera metoden "SetFont" och inte egenskapen "Font". |
| [SetFontColor](../../aspose.cells.griddesktop.data/gridcell/setfontcolor/)(Color) | Sätter teckensnittsfärgen i cellen. För att förbättra prestanda, implementera metoden "SetFontColor" och inte egenskapen "FontColor". |
| [SetFormula](../../aspose.cells.griddesktop.data/gridcell/setformula/)(string, object) | Ange formeln och formelns värde. |
| [SetNumberType](../../aspose.cells.griddesktop.data/gridcell/setnumbertype/)(int) | ange visningsformatet för tal och datum |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcell/setstyle/)(Style) | Ställer in stil för cellen. För att förbättra prestanda, implementera "SetStyle"-metoden, inte implementera "Style"-egenskapen. |
| override [ToString](../../aspose.cells.griddesktop.data/gridcell/tostring/)() | Returnerar en sträng som representerar det aktuella Cell‑objektet. |
| [operator ==](../../aspose.cells.griddesktop.data/gridcell/op_equality/) |  |
| [operator !=](../../aspose.cells.griddesktop.data/gridcell/op_inequality/) |  |

### Se även

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


