---
title: GridCell
second_title: Aspose.Cells för .NET API-referens
description: Representerar ett cellobjekt.
type: docs
weight: 150
url: /sv/net/aspose.cells.gridweb.data/gridcell/
---
## GridCell class

Representerar ett cellobjekt.

```csharp
public class GridCell
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [BoolValue](../../aspose.cells.gridweb.data/gridcell/boolvalue) { get; } | Hämtar det booleska värdet som finns i cellen. |
| [Column](../../aspose.cells.gridweb.data/gridcell/column) { get; } | Hämtar kolumnnummer (nollbaserat) för cellen. |
| [DateValue](../../aspose.cells.gridweb.data/gridcell/datevalue) { get; } | Hämtar DateTime-värdet som finns i cellen. |
| [DisplayStringValue](../../aspose.cells.gridweb.data/gridcell/displaystringvalue) { get; } | Hämtar det formaterade strängvärdet för denna cell. |
| [DoubleValue](../../aspose.cells.gridweb.data/gridcell/doublevalue) { get; } | Får det dubbla värdet som finns i cellen. |
| [FloatValue](../../aspose.cells.gridweb.data/gridcell/floatvalue) { get; } | Hämtar flytvärdet som finns i cellen. |
| [Formula](../../aspose.cells.gridweb.data/gridcell/formula) { get; set; } | Hämtar eller ställer in en formel förCell . |
| [HtmlString](../../aspose.cells.gridweb.data/gridcell/htmlstring) { get; set; } | Hämtar och ställer in html-strängen som innehåller data och vissa formateringar i den här cellen. |
| [IntValue](../../aspose.cells.gridweb.data/gridcell/intvalue) { get; } | Hämtar heltalsvärdet som finns i cellen. |
| [IsStyleSet](../../aspose.cells.gridweb.data/gridcell/isstyleset) { get; } | Indikerar om cellens stil är inställd. Om returnera false betyder det att den här cellen har ett standardcellformat. |
| [Name](../../aspose.cells.gridweb.data/gridcell/name) { get; } | Hämtar namnet på cellen. Till exempel: A1, F102. |
| [Row](../../aspose.cells.gridweb.data/gridcell/row) { get; } | Hämtar radnummer (nollbaserat) för cellen. |
| [StringValue](../../aspose.cells.gridweb.data/gridcell/stringvalue) { get; } | Hämtar strängvärdet som finns i cellen. |
| [Style](../../aspose.cells.gridweb.data/gridcell/style) { get; set; } | Hämtar kopian av cellformat. ställ in stilen för cellen. |
| [Type](../../aspose.cells.gridweb.data/gridcell/type) { get; } | returnerar cellvärdetypen, betydelsen kan se GridCellValueType.java |
| [Value](../../aspose.cells.gridweb.data/gridcell/value) { get; set; } | Hämtar värdet som finns i den här cellen. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [ContainsExternalLink](../../aspose.cells.gridweb.data/gridcell/containsexternallink)() | Indikerar om denna cell innehåller en extern länk. Gäller endast när cellen är en formelcell. |
| [Copy](../../aspose.cells.gridweb.data/gridcell/copy)(GridCell) | Kopierar data från en källcell. |
| [CopyStyle](../../aspose.cells.gridweb.data/gridcell/copystyle)(GridTableItemStyle) | kopiera stilen och ställ in stilen för cell |
| [CreateComment](../../aspose.cells.gridweb.data/gridcell/createcomment)(string, string, bool) | Skapar ett kommentarsobjekt för en cell. |
| [CreateValidation](../../aspose.cells.gridweb.data/gridcell/createvalidation)(GridValidationType, bool) | Skapar ett valideringsobjekt för en cell. |
| override [Equals](../../aspose.cells.gridweb.data/gridcell/equals)(object) |  |
| [GetCellArea](../../aspose.cells.gridweb.data/gridcell/getcellarea)() |  |
| [GetComment](../../aspose.cells.gridweb.data/gridcell/getcomment)() | Få kommentarobjekt på denna cell |
| override [GetHashCode](../../aspose.cells.gridweb.data/gridcell/gethashcode)() |  |
| [GetWidthOfValue](../../aspose.cells.gridweb.data/gridcell/getwidthofvalue)() | Hämtar bredden på värdet i enhet pixlar. |
| [IsErrorValue](../../aspose.cells.gridweb.data/gridcell/iserrorvalue)() | Kontrollerar om en formel korrekt kan utvärdera ett resultat. |
| [IsFormula](../../aspose.cells.gridweb.data/gridcell/isformula)() | Representerar om den angivna cellen innehåller formel. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue)(bool) | Lägger ett booleskt värde i cellen. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_3)(DateTime) | Lägger in ett DateTime-värde i cellen. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_1)(double) | Lägger ett dubbelt värde i cellen. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_2)(int) | Lägger in ett int-värde i cellen. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_4)(object) | Lägger in ett objektvärde i cell.same as setValue(Object param_object) |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_5)(string) | Lägger in ett strängvärde i cellen. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_6)(string, bool) | Lägger in ett strängvärde i cellen och konverterar värdet till annan datatyp om så är lämpligt. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_7)(string, bool, bool) | Lägger in ett värde i cellen, om så är lämpligt kommer värdet att konverteras till annan datatyp och cellens talformat återställs. |
| [PutValueAndSetFormatByValue](../../aspose.cells.gridweb.data/gridcell/putvalueandsetformatbyvalue)(string) | Ställer in cellens värde med ett strängvärde och ställer in cellformat med detta värde. |
| [RemoveComment](../../aspose.cells.gridweb.data/gridcell/removecomment)() | Tar bort kommentarobjektet från cellen. |
| [RemoveValidation](../../aspose.cells.gridweb.data/gridcell/removevalidation)() | Tar bort valideringsobjektet från cellen. |
| [SetBorder](../../aspose.cells.gridweb.data/gridcell/setborder)(WebBorderStyle) | Ställer in kanter (överst, botten, vänster och höger) för en cell, alla kanter har samma kantstil. |
| [SetCustom](../../aspose.cells.gridweb.data/gridcell/setcustom)(string) | ställer in det anpassade formatet, null eller tom sträng betyder inget anpassat format. |
| [SetFormula](../../aspose.cells.gridweb.data/gridcell/setformula)(string, object) | Ställ in formeln och värdet för formeln. |
| [SetNumberType](../../aspose.cells.gridweb.data/gridcell/setnumbertype)(int) | ställ in visningsformatet för siffror och datum |
| [ToString](../../aspose.cells.gridweb.data/gridcell/tostring#tostring)() | Returnerar en sträng som representerar det aktuella cellobjektet. |
| [operator ==](../../aspose.cells.gridweb.data/gridcell/op_equality) |  |
| [operator !=](../../aspose.cells.gridweb.data/gridcell/op_inequality) |  |

### Se även

* namnutrymme [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data)
* hopsättning [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
