---
title: GridCell
second_title: Aspose.Cells für .NET-API-Referenz
description: Repräsentiert ein Zellobjekt.
type: docs
weight: 370
url: /de/net/aspose.cells.griddesktop.data/gridcell/
---
## GridCell class

Repräsentiert ein Zellobjekt.

```csharp
public class GridCell
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BoolValue](../../aspose.cells.griddesktop.data/gridcell/boolvalue) { get; } | Ruft den in der Zelle enthaltenen booleschen Wert ab. |
| [Column](../../aspose.cells.griddesktop.data/gridcell/column) { get; } | Ruft die Spaltennummer (nullbasiert) der Zelle ab. |
| [DateValue](../../aspose.cells.griddesktop.data/gridcell/datevalue) { get; } | Ruft den in der Zelle enthaltenen DateTime-Wert ab. |
| [DisplayStringValue](../../aspose.cells.griddesktop.data/gridcell/displaystringvalue) { get; } | Ruft den formatierten Zeichenfolgenwert dieser Zelle ab. |
| [DoubleValue](../../aspose.cells.griddesktop.data/gridcell/doublevalue) { get; } | Ruft den in der Zelle enthaltenen Double-Wert ab. |
| [FloatValue](../../aspose.cells.griddesktop.data/gridcell/floatvalue) { get; } | Ruft den Float-Wert ab, der in der Zelle enthalten ist. |
| [Formula](../../aspose.cells.griddesktop.data/gridcell/formula) { get; set; } | Ruft eine Formel von ab oder legt sie festCell . |
| [HtmlString](../../aspose.cells.griddesktop.data/gridcell/htmlstring) { get; set; } | Ruft die HTML-Zeichenfolge ab und legt sie fest, die Daten und einige Formatierungen in dieser Zelle enthält. |
| [IntValue](../../aspose.cells.griddesktop.data/gridcell/intvalue) { get; } | Ruft den in der Zelle enthaltenen ganzzahligen Wert ab. |
| [IsStyleSet](../../aspose.cells.griddesktop.data/gridcell/isstyleset) { get; } | Gibt an, ob der Stil der Zelle eingestellt ist. Wenn "false" zurückgegeben wird, bedeutet dies, dass diese Zelle ein Standardzellenformat hat. |
| [Location](../../aspose.cells.griddesktop.data/gridcell/location) { get; } |  |
| [Name](../../aspose.cells.griddesktop.data/gridcell/name) { get; } | Ruft den Namen der Zelle ab. Zum Beispiel: A1, F102. |
| [Protected](../../aspose.cells.griddesktop.data/gridcell/protected) { get; set; } | Gibt an, ob die Zelle geschützt ist. Wenn der Wert "true" ist, kann der Benutzer die Zelle nicht über die Benutzeroberfläche ändern. Dieses Attribut hat nichts mit der Style.CellLocked-Eigenschaft zu tun und wird nicht in einer Datei gespeichert Rasterdaten exportiert. Der Standardwert ist „false“. |
| [Row](../../aspose.cells.griddesktop.data/gridcell/row) { get; } | Ruft die Zeilennummer (nullbasiert) der Zelle ab. |
| [StringValue](../../aspose.cells.griddesktop.data/gridcell/stringvalue) { get; } | Ruft den in der Zelle enthaltenen Zeichenfolgenwert ab. |
| [Style](../../aspose.cells.griddesktop.data/gridcell/style) { get; set; } | Ruft die Kopie des Zellenstils ab. Legen Sie den Stil für die Zelle fest. |
| [Type](../../aspose.cells.griddesktop.data/gridcell/type) { get; } | gibt den Zellwerttyp zurück, die Bedeutung kann GridCellValueType.java entnommen werden |
| [Value](../../aspose.cells.griddesktop.data/gridcell/value) { get; set; } | Ruft den in dieser Zelle enthaltenen Wert ab. |
| [Worksheet](../../aspose.cells.griddesktop.data/gridcell/worksheet) { get; } | Ruft Arbeitsblattobjekt ab. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [ContainsExternalLink](../../aspose.cells.griddesktop.data/gridcell/containsexternallink)() | Gibt an, ob diese Zelle einen externen Link enthält. Gilt nur, wenn die Zelle eine Formelzelle ist. |
| [Copy](../../aspose.cells.griddesktop.data/gridcell/copy)(GridCell) | Kopiert Daten aus einer Quellzelle. |
| [CopyStyle](../../aspose.cells.griddesktop.data/gridcell/copystyle)(Style) | kopiere den Stil und setze den Stil für die Zelle |
| override [Equals](../../aspose.cells.griddesktop.data/gridcell/equals)(object) |  |
| [GetCellArea](../../aspose.cells.griddesktop.data/gridcell/getcellarea)() |  |
| [GetFont](../../aspose.cells.griddesktop.data/gridcell/getfont)() | Ruft die Schriftart der Zelle ab. Wenn Sie die Schriftart ändern, sollten Sie die Methode "SetFont" aufrufen, um die Schriftart auf die Zelle festzulegen. |
| [GetFontColor](../../aspose.cells.griddesktop.data/gridcell/getfontcolor)() | Ruft die Schriftfarbe der Zelle ab. Wenn Sie die Farbe ändern, sollten Sie die Methode "SetFontColor" aufrufen, um die Schriftfarbe auf die Zelle einzustellen. |
| override [GetHashCode](../../aspose.cells.griddesktop.data/gridcell/gethashcode)() |  |
| [GetStyle](../../aspose.cells.griddesktop.data/gridcell/getstyle)() | Ruft den Zellenstil ab. Wenn Sie den Stil ändern, sollten Sie die Methode „SetStyle“ aufrufen, um den Stil auf die Zelle festzulegen. |
| [GetValidation](../../aspose.cells.griddesktop.data/gridcell/getvalidation)() | Ruft die Validierung ab, die auf diese Zelle angewendet wurde. Wenn nicht gesetzt, wird null zurückgegeben. |
| [GetWidthOfValue](../../aspose.cells.griddesktop.data/gridcell/getwidthofvalue)() | Ruft die Breite des Werts in Pixeleinheiten ab. |
| [GetWorksheet](../../aspose.cells.griddesktop.data/gridcell/getworksheet)() | Ruft das übergeordnete Arbeitsblatt ab. |
| [IsErrorValue](../../aspose.cells.griddesktop.data/gridcell/iserrorvalue)() | Prüft, ob eine Formel ein Ergebnis richtig auswerten kann. |
| [IsFormula](../../aspose.cells.griddesktop.data/gridcell/isformula)() | Stellt dar, ob die angegebene Zelle eine Formel enthält. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue)(bool) | Fügt einen booleschen Wert in die Zelle ein. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_3)(DateTime) | Fügt einen DateTime-Wert in die Zelle ein. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_1)(double) | Fügt einen doppelten Wert in die Zelle ein. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_2)(int) | Fügt einen int-Wert in die Zelle ein. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_4)(object) | Fügt einen Objektwert in die Zelle ein. Dasselbe wie setValue(Object param_object) |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_5)(string) | Fügt einen String-Wert in die Zelle ein. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_6)(string, bool) | Fügt einen Zeichenfolgenwert in die Zelle ein und konvertiert den Wert gegebenenfalls in einen anderen Datentyp. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_7)(string, bool, bool) | Fügt einen Wert in die Zelle ein, gegebenenfalls wird der Wert in einen anderen Datentyp konvertiert und das Zahlenformat der Zelle wird zurückgesetzt. |
| [PutValueAndSetFormatByValue](../../aspose.cells.griddesktop.data/gridcell/putvalueandsetformatbyvalue)(string) | Legt den Wert der Zelle mit einem Zeichenfolgenwert fest und legt das Zellenformat mit diesem Wert fest. |
| [SetCellValue](../../aspose.cells.griddesktop.data/gridcell/setcellvalue)(object) | Wenn der Wert eine Formel ist, setzt diese Methode den Wert der Zelle als FormulaType, |
| [SetCustom](../../aspose.cells.griddesktop.data/gridcell/setcustom)(string) | legt das benutzerdefinierte Format fest, null oder leere Zeichenfolge bedeutet kein benutzerdefiniertes Format. |
| [SetFont](../../aspose.cells.griddesktop.data/gridcell/setfont)(Font) | Legt die Schriftart für die Zelle fest. Um die Leistung zu verbessern, implementieren Sie die Methode „SetFont“, implementieren Sie die Eigenschaft „Font“ nicht. |
| [SetFontColor](../../aspose.cells.griddesktop.data/gridcell/setfontcolor)(Color) | Legt die Schriftfarbe für die Zelle fest. Um die Leistung zu verbessern, implementieren Sie die Methode "SetFontColor", implementieren Sie die Eigenschaft "FontColor" nicht. |
| [SetFormula](../../aspose.cells.griddesktop.data/gridcell/setformula)(string, object) | Stellen Sie die Formel und den Wert der Formel ein. |
| [SetNumberType](../../aspose.cells.griddesktop.data/gridcell/setnumbertype)(int) | stellt das Anzeigeformat von Zahlen und Daten ein |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcell/setstyle)(Style) | Legt den Stil auf die Zelle fest. Um die Leistung zu verbessern, implementieren Sie die Methode "SetStyle", implementieren Sie die Eigenschaft "Style" nicht. |
| [ToString](../../aspose.cells.griddesktop.data/gridcell/tostring#tostring)() | Gibt eine Zeichenfolge zurück, die das aktuelle Cell-Objekt darstellt. |
| [operator ==](../../aspose.cells.griddesktop.data/gridcell/op_equality) |  |
| [operator !=](../../aspose.cells.griddesktop.data/gridcell/op_inequality) |  |

### Siehe auch

* namensraum [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data)
* Montage [Aspose.Cells.GridDesktop](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
