---
title: "Klasse GridCell"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridWeb.Data.GridCell Klasse. Stellt ein Zellenobjekt dar"
type: docs
url: /de/net/aspose.cells.gridweb.data/gridcell/
---
## GridCell class

Stellt ein Zellenobjekt dar.

```csharp
public class GridCell
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BoolValue](../../aspose.cells.gridweb.data/gridcell/boolvalue/) { get; } | Liefert den booleschen Wert, der in der Zelle enthalten ist. |
| [Column](../../aspose.cells.gridweb.data/gridcell/column/) { get; } | Liefert die Spaltennummer (nullbasiert) der Zelle. |
| [DateValue](../../aspose.cells.gridweb.data/gridcell/datevalue/) { get; } | Liefert den DateTime-Wert, der in der Zelle enthalten ist. |
| [DisplayStringValue](../../aspose.cells.gridweb.data/gridcell/displaystringvalue/) { get; } | Liest den formatierten Zeichenkettenwert dieser Zelle. |
| [DoubleValue](../../aspose.cells.gridweb.data/gridcell/doublevalue/) { get; } | Liefert den double-Wert, der in der Zelle enthalten ist. |
| [FloatValue](../../aspose.cells.gridweb.data/gridcell/floatvalue/) { get; } | Liefert den float-Wert, der in der Zelle enthalten ist. |
| [Formula](../../aspose.cells.gridweb.data/gridcell/formula/) { get; set; } | Liest oder setzt eine Formel des `GridCell`. |
| [HtmlString](../../aspose.cells.gridweb.data/gridcell/htmlstring/) { get; set; } | Liest und setzt die HTML-Zeichenkette, die Daten und einige Formatierungen in dieser Zelle enthält. |
| [IntValue](../../aspose.cells.gridweb.data/gridcell/intvalue/) { get; } | Liefert den ganzzahligen Wert, der in der Zelle enthalten ist. |
| [IsStyleSet](../../aspose.cells.gridweb.data/gridcell/isstyleset/) { get; } | Gibt an, ob der Zellenstil festgelegt ist. Wenn false zurückgegeben wird, bedeutet dies, dass diese Zelle ein Standardzellenformat hat. |
| [Name](../../aspose.cells.gridweb.data/gridcell/name/) { get; } | Liest den Namen der Zelle. Zum Beispiel: A1, F102. |
| [Row](../../aspose.cells.gridweb.data/gridcell/row/) { get; } | Ermittelt die Zeilennummer (nullbasiert) der Zelle. |
| [StringValue](../../aspose.cells.gridweb.data/gridcell/stringvalue/) { get; } | Liest den Zeichenkettenwert, der in der Zelle enthalten ist. |
| [Style](../../aspose.cells.gridweb.data/gridcell/style/) { get; set; } | Liest die Kopie des Zellenstils. Setzt den Stil für die Zelle. |
| [Type](../../aspose.cells.gridweb.data/gridcell/type/) { get; } | Gibt den Zellenwerttyp zurück, die Bedeutung kann in GridCellValueType.java nachgelesen werden. |
| [Value](../../aspose.cells.gridweb.data/gridcell/value/) { get; set; } | Liest den in dieser Zelle enthaltenen Wert. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [ContainsExternalLink](../../aspose.cells.gridweb.data/gridcell/containsexternallink/)() | Gibt an, ob diese Zelle einen externen Link enthält. Gilt nur, wenn die Zelle eine Formelzelle ist. |
| [Copy](../../aspose.cells.gridweb.data/gridcell/copy/)(GridCell) | Kopiert Daten aus einer Quellzelle. |
| [CopyStyle](../../aspose.cells.gridweb.data/gridcell/copystyle/)(GridTableItemStyle) | Kopiere den Stil und setze den Stil für die Zelle. |
| [CreateComment](../../aspose.cells.gridweb.data/gridcell/createcomment/)(string, string, bool) | Erstellt ein Kommentarobjekt für eine Zelle. |
| [CreateValidation](../../aspose.cells.gridweb.data/gridcell/createvalidation/)(GridValidationType, bool) | Erstellt ein Validierungsobjekt für eine Zelle. |
| override [Equals](../../aspose.cells.gridweb.data/gridcell/equals/)(object) | Prüft, ob dieses Objekt auf dieselbe Zelle wie ein anderes Zellenobjekt verweist. |
| [GetComment](../../aspose.cells.gridweb.data/gridcell/getcomment/)() | Kommentarobjekt dieser Zelle abrufen |
| override [GetHashCode](../../aspose.cells.gridweb.data/gridcell/gethashcode/)() | Dient als Hash-Funktion für einen bestimmten Typ. |
| [GetWidthOfValue](../../aspose.cells.gridweb.data/gridcell/getwidthofvalue/)() | Liefert die Breite des Werts in der Einheit Pixel. |
| [IsErrorValue](../../aspose.cells.gridweb.data/gridcell/iserrorvalue/)() | Überprüft, ob eine Formel ein Ergebnis korrekt auswerten kann. |
| [IsFormula](../../aspose.cells.gridweb.data/gridcell/isformula/)() | Gibt an, ob die angegebene Zelle eine Formel enthält. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue)(bool) | Schreibt einen booleschen Wert in die Zelle. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_3)(DateTime) | Schreibt einen DateTime‑Wert in die Zelle. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_1)(double) | Schreibt einen double‑Wert in die Zelle. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_2)(int) | Setzt einen int‑Wert in die Zelle. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_4)(object) | Setzt einen Objektwert in die Zelle. Gleichbedeutend mit setValue(Object param_object) |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_5)(string) | Setzt einen String‑Wert in die Zelle. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_6)(string, bool) | Fügt einen Zeichenkettenwert in die Zelle ein und konvertiert den Wert bei Bedarf in einen anderen Datentyp. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_7)(string, bool, bool) | Fügt einen Wert in die Zelle ein, bei Bedarf wird der Wert in einen anderen Datentyp konvertiert und das Zahlenformat der Zelle zurückgesetzt. |
| [PutValueAndSetFormatByValue](../../aspose.cells.gridweb.data/gridcell/putvalueandsetformatbyvalue/)(string) | Setzt den Zellenwert mit einem Zeichenkettenwert und legt das Zellenformat anhand dieses Werts fest. |
| [RemoveComment](../../aspose.cells.gridweb.data/gridcell/removecomment/)() | Entfernt das Kommentarobjekt der Zelle. |
| [RemoveValidation](../../aspose.cells.gridweb.data/gridcell/removevalidation/)() | Entfernt das Validierungsobjekt der Zelle. |
| [SetBorder](../../aspose.cells.gridweb.data/gridcell/setborder/)(WebBorderStyle) | Setzt Rahmen (oben, unten, links und rechts) für eine Zelle, alle Rahmen haben denselben Rahmenstil. |
| [SetCustom](../../aspose.cells.gridweb.data/gridcell/setcustom/)(string) | Setzt das benutzerdefinierte Format, null oder ein leerer String bedeutet kein benutzerdefiniertes Format. |
| [SetFormula](../../aspose.cells.gridweb.data/gridcell/setformula/)(string, object) | Setzt die Formel und den Wert der Formel. |
| [SetNumberType](../../aspose.cells.gridweb.data/gridcell/setnumbertype/)(int) | Setzt das Anzeigeformat von Zahlen und Datumsangaben |
| [ToString](../../aspose.cells.gridweb.data/gridcell/tostring/#tostring)() | Gibt eine Zeichenkette zurück, die das aktuelle Cell-Objekt darstellt. |
| [operator ==](../../aspose.cells.gridweb.data/gridcell/op_equality/) |  |
| [operator !=](../../aspose.cells.gridweb.data/gridcell/op_inequality/) |  |

### Siehe auch

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


