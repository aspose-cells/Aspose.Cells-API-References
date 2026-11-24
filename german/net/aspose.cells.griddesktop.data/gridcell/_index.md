---
title: "Klasse GridCell"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridDesktop.Data.GridCell Klasse. Stellt ein Zellenobjekt dar"
type: docs
url: /de/net/aspose.cells.griddesktop.data/gridcell/
---
## GridCell class

Stellt ein Zellenobjekt dar.

```csharp
public class GridCell
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BoolValue](../../aspose.cells.griddesktop.data/gridcell/boolvalue/) { get; } | Liefert den booleschen Wert, der in der Zelle enthalten ist. |
| [Column](../../aspose.cells.griddesktop.data/gridcell/column/) { get; } | Liefert die Spaltennummer (nullbasiert) der Zelle. |
| [DateValue](../../aspose.cells.griddesktop.data/gridcell/datevalue/) { get; } | Liefert den DateTime-Wert, der in der Zelle enthalten ist. |
| [DisplayStringValue](../../aspose.cells.griddesktop.data/gridcell/displaystringvalue/) { get; } | Liest den formatierten Zeichenkettenwert dieser Zelle. |
| [DoubleValue](../../aspose.cells.griddesktop.data/gridcell/doublevalue/) { get; } | Liefert den double-Wert, der in der Zelle enthalten ist. |
| [FloatValue](../../aspose.cells.griddesktop.data/gridcell/floatvalue/) { get; } | Liefert den float-Wert, der in der Zelle enthalten ist. |
| [Formula](../../aspose.cells.griddesktop.data/gridcell/formula/) { get; set; } | Liest oder setzt eine Formel der Zelle. |
| [HasCustomStyle](../../aspose.cells.griddesktop.data/gridcell/hascustomstyle/) { get; } | Gibt an, ob diese Zelle benutzerdefinierte Stileinstellungen hat (anders als die Standard‑Einstellungen, die von der entsprechenden Zeile, Spalte oder Arbeitsmappe geerbt werden). |
| [HtmlString](../../aspose.cells.griddesktop.data/gridcell/htmlstring/) { get; set; } | Liest und setzt die HTML-Zeichenkette, die Daten und einige Formatierungen in dieser Zelle enthält. |
| [IntValue](../../aspose.cells.griddesktop.data/gridcell/intvalue/) { get; } | Liefert den ganzzahligen Wert, der in der Zelle enthalten ist. |
| [IsStyleSet](../../aspose.cells.griddesktop.data/gridcell/isstyleset/) { get; } | Gibt an, ob der Zellenstil festgelegt ist. Wenn false zurückgegeben wird, bedeutet dies, dass diese Zelle ein Standardzellenformat hat. |
| [Location](../../aspose.cells.griddesktop.data/gridcell/location/) { get; } |  |
| [Name](../../aspose.cells.griddesktop.data/gridcell/name/) { get; } | Liest den Namen der Zelle. Zum Beispiel: A1, F102. |
| [Protected](../../aspose.cells.griddesktop.data/gridcell/protected/) { get; set; } | Gibt an, ob die Zelle geschützt ist. Wenn der Wert "true" ist, kann der Benutzer die Zelle nicht über die Benutzeroberfläche ändern. Dieses Attribut hat nichts mit der Style.CellLocked‑Eigenschaft zu tun und wird beim Export von Gitterdaten nicht in die Datei gespeichert. Der Standardwert ist "false". |
| [Row](../../aspose.cells.griddesktop.data/gridcell/row/) { get; } | Ermittelt die Zeilennummer (nullbasiert) der Zelle. |
| [StringValue](../../aspose.cells.griddesktop.data/gridcell/stringvalue/) { get; } | Liest den Zeichenkettenwert, der in der Zelle enthalten ist. |
| [Style](../../aspose.cells.griddesktop.data/gridcell/style/) { get; set; } | Liest die Kopie des Zellenstils. Setzt den Stil für die Zelle. |
| [Type](../../aspose.cells.griddesktop.data/gridcell/type/) { get; } | Gibt den Zellenwerttyp zurück, die Bedeutung kann in GridCellValueType.java nachgelesen werden. |
| [Value](../../aspose.cells.griddesktop.data/gridcell/value/) { get; set; } | Liest den in dieser Zelle enthaltenen Wert. |
| [Worksheet](../../aspose.cells.griddesktop.data/gridcell/worksheet/) { get; } | Liest das Arbeitsblattobjekt. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [ContainsExternalLink](../../aspose.cells.griddesktop.data/gridcell/containsexternallink/)() | Gibt an, ob diese Zelle einen externen Link enthält. Gilt nur, wenn die Zelle eine Formelzelle ist. |
| [Copy](../../aspose.cells.griddesktop.data/gridcell/copy/)(GridCell) | Kopiert Daten aus einer Quellzelle. |
| [CopyStyle](../../aspose.cells.griddesktop.data/gridcell/copystyle/)(Style) | Kopiere den Stil und setze den Stil für die Zelle. |
| override [Equals](../../aspose.cells.griddesktop.data/gridcell/equals/)(object) |  |
| [GetCellArea](../../aspose.cells.griddesktop.data/gridcell/getcellarea/)() |  |
| [GetFont](../../aspose.cells.griddesktop.data/gridcell/getfont/)() | Liest die Zellen­schriftart. Wenn die Schriftart geändert wird, sollten Sie die Methode "SetFont" aufrufen, um die Schriftart für die Zelle festzulegen. |
| [GetFontColor](../../aspose.cells.griddesktop.data/gridcell/getfontcolor/)() | Liest die Schriftfarbe der Zelle. Wenn die Farbe geändert wird, sollten Sie die Methode "SetFontColor" aufrufen, um die Schriftfarbe für die Zelle festzulegen. |
| override [GetHashCode](../../aspose.cells.griddesktop.data/gridcell/gethashcode/)() |  |
| [GetStyle](../../aspose.cells.griddesktop.data/gridcell/getstyle/)() | Liest den Zellenstil. Wenn der Stil geändert wird, sollten Sie die Methode "SetStyle" aufrufen, um den Stil für die Zelle festzulegen. |
| [GetValidation](../../aspose.cells.griddesktop.data/gridcell/getvalidation/)() | Liest die Validierung, die für diese Zelle angewendet wird. Wenn nicht gesetzt, wird null zurückgegeben. |
| [GetWidthOfValue](../../aspose.cells.griddesktop.data/gridcell/getwidthofvalue/)() | Liefert die Breite des Werts in der Einheit Pixel. |
| [GetWorksheet](../../aspose.cells.griddesktop.data/gridcell/getworksheet/)() | Ermittelt das übergeordnete Arbeitsblatt. |
| [IsErrorValue](../../aspose.cells.griddesktop.data/gridcell/iserrorvalue/)() | Überprüft, ob eine Formel ein Ergebnis korrekt auswerten kann. |
| [IsFormula](../../aspose.cells.griddesktop.data/gridcell/isformula/)() | Gibt an, ob die angegebene Zelle eine Formel enthält. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue)(bool) | Schreibt einen booleschen Wert in die Zelle. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_3)(DateTime) | Schreibt einen DateTime‑Wert in die Zelle. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_1)(double) | Schreibt einen double‑Wert in die Zelle. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_2)(int) | Setzt einen int‑Wert in die Zelle. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_4)(object) | Setzt einen Objektwert in die Zelle. Gleichbedeutend mit setValue(Object param_object) |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_5)(string) | Setzt einen String‑Wert in die Zelle. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_6)(string, bool) | Fügt einen Zeichenkettenwert in die Zelle ein und konvertiert den Wert bei Bedarf in einen anderen Datentyp. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_7)(string, bool, bool) | Fügt einen Wert in die Zelle ein, bei Bedarf wird der Wert in einen anderen Datentyp konvertiert und das Zahlenformat der Zelle zurückgesetzt. |
| [PutValueAndSetFormatByValue](../../aspose.cells.griddesktop.data/gridcell/putvalueandsetformatbyvalue/)(string) | Setzt den Zellenwert mit einem Zeichenkettenwert und legt das Zellenformat anhand dieses Werts fest. |
| [SetCellValue](../../aspose.cells.griddesktop.data/gridcell/setcellvalue/)(object) | Wenn der Wert eine Formel ist, setzt diese Methode den Zellenwert als FormulaType, |
| [SetCustom](../../aspose.cells.griddesktop.data/gridcell/setcustom/)(string) | Setzt das benutzerdefinierte Format, null oder ein leerer String bedeutet kein benutzerdefiniertes Format. |
| [SetFont](../../aspose.cells.griddesktop.data/gridcell/setfont/)(Font) | Setzt die Schriftart für die Zelle. Um die Leistung zu verbessern, implementieren Sie die Methode "SetFont", nicht die Eigenschaft "Font". |
| [SetFontColor](../../aspose.cells.griddesktop.data/gridcell/setfontcolor/)(Color) | Setzt die Schriftfarbe für die Zelle. Um die Leistung zu verbessern, implementieren Sie die Methode "SetFontColor", nicht die Eigenschaft "FontColor". |
| [SetFormula](../../aspose.cells.griddesktop.data/gridcell/setformula/)(string, object) | Setzt die Formel und den Wert der Formel. |
| [SetNumberType](../../aspose.cells.griddesktop.data/gridcell/setnumbertype/)(int) | Setzt das Anzeigeformat von Zahlen und Datumsangaben |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcell/setstyle/)(Style) | Setzt den Stil für die Zelle. Um die Leistung zu verbessern, implementieren Sie die Methode "SetStyle", nicht die Eigenschaft "Style". |
| override [ToString](../../aspose.cells.griddesktop.data/gridcell/tostring/)() | Gibt eine Zeichenkette zurück, die das aktuelle Cell-Objekt darstellt. |
| [operator ==](../../aspose.cells.griddesktop.data/gridcell/op_equality/) |  |
| [operator !=](../../aspose.cells.griddesktop.data/gridcell/op_inequality/) |  |

### Siehe auch

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


