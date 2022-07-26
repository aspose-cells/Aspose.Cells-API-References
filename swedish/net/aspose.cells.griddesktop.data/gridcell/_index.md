---
title: GridCell
second_title: Aspose.Cells för .NET API-referens
description: Representerar ett cellobjekt.
type: docs
weight: 370
url: /sv/net/aspose.cells.griddesktop.data/gridcell/
---
## GridCell class

Representerar ett cellobjekt.

```csharp
public class GridCell
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [BoolValue](../../aspose.cells.griddesktop.data/gridcell/boolvalue) { get; } | Hämtar det booleska värdet som finns i cellen. |
| [Column](../../aspose.cells.griddesktop.data/gridcell/column) { get; } | Hämtar kolumnnummer (nollbaserat) för cellen. |
| [DateValue](../../aspose.cells.griddesktop.data/gridcell/datevalue) { get; } | Hämtar DateTime-värdet som finns i cellen. |
| [DisplayStringValue](../../aspose.cells.griddesktop.data/gridcell/displaystringvalue) { get; } | Hämtar det formaterade strängvärdet för denna cell. |
| [DoubleValue](../../aspose.cells.griddesktop.data/gridcell/doublevalue) { get; } | Får det dubbla värdet som finns i cellen. |
| [FloatValue](../../aspose.cells.griddesktop.data/gridcell/floatvalue) { get; } | Hämtar flytvärdet som finns i cellen. |
| [Formula](../../aspose.cells.griddesktop.data/gridcell/formula) { get; set; } | Hämtar eller ställer in en formel förCell . |
| [HtmlString](../../aspose.cells.griddesktop.data/gridcell/htmlstring) { get; set; } | Hämtar och ställer in html-strängen som innehåller data och vissa formateringar i den här cellen. |
| [IntValue](../../aspose.cells.griddesktop.data/gridcell/intvalue) { get; } | Hämtar heltalsvärdet som finns i cellen. |
| [IsStyleSet](../../aspose.cells.griddesktop.data/gridcell/isstyleset) { get; } | Indikerar om cellens stil är inställd. Om returnera false betyder det att den här cellen har ett standardcellformat. |
| [Location](../../aspose.cells.griddesktop.data/gridcell/location) { get; } |  |
| [Name](../../aspose.cells.griddesktop.data/gridcell/name) { get; } | Hämtar namnet på cellen. Till exempel: A1, F102. |
| [Protected](../../aspose.cells.griddesktop.data/gridcell/protected) { get; set; } | Indikerar om cellen är skyddad. Om värdet är "true" kan användaren inte ändra cellen via användargränssnittet. Det här attributet har inget att göra med Style.CellLocked-egenskapen och kommer inte att sparas i filen när rutnätsdata exporterad. Standardvärdet är "false". |
| [Row](../../aspose.cells.griddesktop.data/gridcell/row) { get; } | Hämtar radnummer (nollbaserat) för cellen. |
| [StringValue](../../aspose.cells.griddesktop.data/gridcell/stringvalue) { get; } | Hämtar strängvärdet som finns i cellen. |
| [Style](../../aspose.cells.griddesktop.data/gridcell/style) { get; set; } | Hämtar kopian av cellformat. ställ in stilen för cellen. |
| [Type](../../aspose.cells.griddesktop.data/gridcell/type) { get; } | returnerar cellvärdetypen, betydelsen kan se GridCellValueType.java |
| [Value](../../aspose.cells.griddesktop.data/gridcell/value) { get; set; } | Hämtar värdet som finns i den här cellen. |
| [Worksheet](../../aspose.cells.griddesktop.data/gridcell/worksheet) { get; } | Hämtar kalkylbladsobjekt. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [ContainsExternalLink](../../aspose.cells.griddesktop.data/gridcell/containsexternallink)() | Indikerar om denna cell innehåller en extern länk. Gäller endast när cellen är en formelcell. |
| [Copy](../../aspose.cells.griddesktop.data/gridcell/copy)(GridCell) | Kopierar data från en källcell. |
| [CopyStyle](../../aspose.cells.griddesktop.data/gridcell/copystyle)(Style) | kopiera stilen och ställ in stilen för cell |
| override [Equals](../../aspose.cells.griddesktop.data/gridcell/equals)(object) |  |
| [GetCellArea](../../aspose.cells.griddesktop.data/gridcell/getcellarea)() |  |
| [GetFont](../../aspose.cells.griddesktop.data/gridcell/getfont)() | Hämtar celltypsnitt. När du ändrar teckensnitt bör du anropa "SetFont"-metoden, för att ställa in teckensnitt till cell. |
| [GetFontColor](../../aspose.cells.griddesktop.data/gridcell/getfontcolor)() | Får cellteckensnittsfärg. När du ändrar färgen bör du anropa "SetFontColor"-metoden, för att ställa in teckensnittsfärgen till cell. |
| override [GetHashCode](../../aspose.cells.griddesktop.data/gridcell/gethashcode)() |  |
| [GetStyle](../../aspose.cells.griddesktop.data/gridcell/getstyle)() | Får cellstil. När du ändrar stil bör du anropa "SetStyle"-metoden, för att ställa in stil till cell. |
| [GetValidation](../../aspose.cells.griddesktop.data/gridcell/getvalidation)() | Får valideringen som gällde för denna cell.if not set return null. |
| [GetWidthOfValue](../../aspose.cells.griddesktop.data/gridcell/getwidthofvalue)() | Hämtar bredden på värdet i enhet pixlar. |
| [GetWorksheet](../../aspose.cells.griddesktop.data/gridcell/getworksheet)() | Hämtar det överordnade arbetsbladet. |
| [IsErrorValue](../../aspose.cells.griddesktop.data/gridcell/iserrorvalue)() | Kontrollerar om en formel korrekt kan utvärdera ett resultat. |
| [IsFormula](../../aspose.cells.griddesktop.data/gridcell/isformula)() | Representerar om den angivna cellen innehåller formel. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue)(bool) | Lägger ett booleskt värde i cellen. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_3)(DateTime) | Lägger in ett DateTime-värde i cellen. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_1)(double) | Lägger ett dubbelt värde i cellen. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_2)(int) | Lägger in ett int-värde i cellen. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_4)(object) | Lägger in ett objektvärde i cell.same as setValue(Object param_object) |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_5)(string) | Lägger in ett strängvärde i cellen. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_6)(string, bool) | Lägger in ett strängvärde i cellen och konverterar värdet till annan datatyp om så är lämpligt. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_7)(string, bool, bool) | Lägger in ett värde i cellen, om så är lämpligt kommer värdet att konverteras till annan datatyp och cellens talformat återställs. |
| [PutValueAndSetFormatByValue](../../aspose.cells.griddesktop.data/gridcell/putvalueandsetformatbyvalue)(string) | Ställer in cellens värde med ett strängvärde och ställer in cellformat med detta värde. |
| [SetCellValue](../../aspose.cells.griddesktop.data/gridcell/setcellvalue)(object) | Om värdet är en formel, ställer den här metoden in cellens värde som FormulaType, |
| [SetCustom](../../aspose.cells.griddesktop.data/gridcell/setcustom)(string) | ställer in det anpassade formatet, null eller tom sträng betyder inget anpassat format. |
| [SetFont](../../aspose.cells.griddesktop.data/gridcell/setfont)(Font) | Anger teckensnitt till cell. För att förbättra prestanda, implementera "SetFont"-metoden, implementera inte egenskapen "Font". |
| [SetFontColor](../../aspose.cells.griddesktop.data/gridcell/setfontcolor)(Color) | Anger teckensnittsfärg till cell. För att förbättra prestanda, implementera "SetFontColor"-metoden, implementera inte egenskapen "FontColor". |
| [SetFormula](../../aspose.cells.griddesktop.data/gridcell/setformula)(string, object) | Ställ in formeln och värdet för formeln. |
| [SetNumberType](../../aspose.cells.griddesktop.data/gridcell/setnumbertype)(int) | ställ in visningsformatet för siffror och datum |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcell/setstyle)(Style) | Anger stil till cell. För att förbättra prestandan, implementera "SetStyle"-metoden, implementera inte "Style"-egenskapen. |
| [ToString](../../aspose.cells.griddesktop.data/gridcell/tostring#tostring)() | Returnerar en sträng som representerar det aktuella cellobjektet. |
| [operator ==](../../aspose.cells.griddesktop.data/gridcell/op_equality) |  |
| [operator !=](../../aspose.cells.griddesktop.data/gridcell/op_inequality) |  |

### Se även

* namnutrymme [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data)
* hopsättning [Aspose.Cells.GridDesktop](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
