---
title: "Klass GridCell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridWeb.Data.GridCell-klass. Representerar ett cellobjekt"
type: docs
url: /sv/net/aspose.cells.gridweb.data/gridcell/
---
## GridCell class

Representerar ett cellobjekt.

```csharp
public class GridCell
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [BoolValue](../../aspose.cells.gridweb.data/gridcell/boolvalue/) { get; } | Hämtar det booleska värdet som finns i cellen. |
| [Column](../../aspose.cells.gridweb.data/gridcell/column/) { get; } | Hämtar kolumnnumret (nollbaserat) för cellen. |
| [DateValue](../../aspose.cells.gridweb.data/gridcell/datevalue/) { get; } | Hämtar DateTime‑värdet som finns i cellen. |
| [DisplayStringValue](../../aspose.cells.gridweb.data/gridcell/displaystringvalue/) { get; } | Hämtar det formaterade strängvärdet för den här cellen. |
| [DoubleValue](../../aspose.cells.gridweb.data/gridcell/doublevalue/) { get; } | Hämtar dubbelvärdet som finns i cellen. |
| [FloatValue](../../aspose.cells.gridweb.data/gridcell/floatvalue/) { get; } | Hämtar flyttalsvärdet som finns i cellen. |
| [Formula](../../aspose.cells.gridweb.data/gridcell/formula/) { get; set; } | Hämtar eller anger en formel för `GridCell`. |
| [HtmlString](../../aspose.cells.gridweb.data/gridcell/htmlstring/) { get; set; } | Hämtar och anger HTML-strängen som innehåller data och viss formatering i den här cellen. |
| [IntValue](../../aspose.cells.gridweb.data/gridcell/intvalue/) { get; } | Hämtar heltalsvärdet som finns i cellen. |
| [IsStyleSet](../../aspose.cells.gridweb.data/gridcell/isstyleset/) { get; } | Anger om cellens stil är angiven. Om den returnerar false betyder det att cellen har ett standardformat. |
| [Name](../../aspose.cells.gridweb.data/gridcell/name/) { get; } | Hämtar namnet på cellen. Till exempel: A1, F102. |
| [Row](../../aspose.cells.gridweb.data/gridcell/row/) { get; } | Hämtar radnumret (nollbaserat) för cellen. |
| [StringValue](../../aspose.cells.gridweb.data/gridcell/stringvalue/) { get; } | Hämtar strängvärdet som finns i cellen. |
| [Style](../../aspose.cells.gridweb.data/gridcell/style/) { get; set; } | Hämtar en kopia av cellstilen. Ange stilen för cellen. |
| [Type](../../aspose.cells.gridweb.data/gridcell/type/) { get; } | returnerar cellvärdestypen, betydelsen kan ses i GridCellValueType.java |
| [Value](../../aspose.cells.gridweb.data/gridcell/value/) { get; set; } | Hämtar värdet som finns i den här cellen. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [ContainsExternalLink](../../aspose.cells.gridweb.data/gridcell/containsexternallink/)() | Anger om den här cellen innehåller en extern länk. Gäller endast när cellen är en formelcell. |
| [Copy](../../aspose.cells.gridweb.data/gridcell/copy/)(GridCell) | Kopierar data från en källcell. |
| [CopyStyle](../../aspose.cells.gridweb.data/gridcell/copystyle/)(GridTableItemStyle) | kopiera stilen och ange stilen för cellen |
| [CreateComment](../../aspose.cells.gridweb.data/gridcell/createcomment/)(string, string, bool) | Skapar ett kommentarsobjekt för en cell. |
| [CreateValidation](../../aspose.cells.gridweb.data/gridcell/createvalidation/)(GridValidationType, bool) | Skapar ett valideringsobjekt för en cell. |
| override [Equals](../../aspose.cells.gridweb.data/gridcell/equals/)(object) | Kontrollerar om detta objekt refererar till samma cell som ett annat cellobjekt. |
| [GetComment](../../aspose.cells.gridweb.data/gridcell/getcomment/)() | Hämta kommentarsobjekt på denna cell |
| override [GetHashCode](../../aspose.cells.gridweb.data/gridcell/gethashcode/)() | Fungerar som en hash-funktion för en viss typ. |
| [GetWidthOfValue](../../aspose.cells.gridweb.data/gridcell/getwidthofvalue/)() | Hämtar bredden på värdet i enheten pixlar. |
| [IsErrorValue](../../aspose.cells.gridweb.data/gridcell/iserrorvalue/)() | Kontrollerar om en formel kan utvärdera ett resultat korrekt. |
| [IsFormula](../../aspose.cells.gridweb.data/gridcell/isformula/)() | Anger om den angivna cellen innehåller en formel. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue)(bool) | Sätter ett booleskt värde i cellen. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_3)(DateTime) | Sätter ett DateTime-värde i cellen. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_1)(double) | Sätter ett double-värde i cellen. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_2)(int) | Sätter ett heltalsvärde i cellen. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_4)(object) | Sätter ett objektvärde i cellen. Samma som setValue(Object param_object) |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_5)(string) | Sätter ett strängvärde i cellen. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_6)(string, bool) | Sätter ett strängvärde i cellen och konverterar värdet till annan datatyp om lämpligt. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_7)(string, bool, bool) | Sätter ett värde i cellen, om lämpligt kommer värdet att konverteras till annan datatyp och cellens talformat återställas. |
| [PutValueAndSetFormatByValue](../../aspose.cells.gridweb.data/gridcell/putvalueandsetformatbyvalue/)(string) | Sätter cellens värde med ett strängvärde och anger cellformatet baserat på detta värde. |
| [RemoveComment](../../aspose.cells.gridweb.data/gridcell/removecomment/)() | Tar bort kommentarsobjektet för cellen. |
| [RemoveValidation](../../aspose.cells.gridweb.data/gridcell/removevalidation/)() | Tar bort valideringsobjektet för cellen. |
| [SetBorder](../../aspose.cells.gridweb.data/gridcell/setborder/)(WebBorderStyle) | Ställer in kanter (övre, nedre, vänstra och högra) för en cell, alla kanter har samma kantstil. |
| [SetCustom](../../aspose.cells.gridweb.data/gridcell/setcustom/)(string) | sätter det anpassade formatet, null eller tom sträng betyder inget anpassat format. |
| [SetFormula](../../aspose.cells.gridweb.data/gridcell/setformula/)(string, object) | Ange formeln och formelns värde. |
| [SetNumberType](../../aspose.cells.gridweb.data/gridcell/setnumbertype/)(int) | ange visningsformatet för tal och datum |
| [ToString](../../aspose.cells.gridweb.data/gridcell/tostring/#tostring)() | Returnerar en sträng som representerar det aktuella Cell‑objektet. |
| [operator ==](../../aspose.cells.gridweb.data/gridcell/op_equality/) |  |
| [operator !=](../../aspose.cells.gridweb.data/gridcell/op_inequality/) |  |

### Se även

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


