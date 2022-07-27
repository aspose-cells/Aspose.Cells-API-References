---
title: GridCell
second_title: Aspose.Cells für .NET-API-Referenz
description: Repräsentiert ein Zellobjekt.
type: docs
weight: 150
url: /de/net/aspose.cells.gridweb.data/gridcell/
---
## GridCell class

Repräsentiert ein Zellobjekt.

```csharp
public class GridCell
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BoolValue](../../aspose.cells.gridweb.data/gridcell/boolvalue) { get; } | Ruft den in der Zelle enthaltenen booleschen Wert ab. |
| [Column](../../aspose.cells.gridweb.data/gridcell/column) { get; } | Ruft die Spaltennummer (nullbasiert) der Zelle ab. |
| [DateValue](../../aspose.cells.gridweb.data/gridcell/datevalue) { get; } | Ruft den in der Zelle enthaltenen DateTime-Wert ab. |
| [DisplayStringValue](../../aspose.cells.gridweb.data/gridcell/displaystringvalue) { get; } | Ruft den formatierten Zeichenfolgenwert dieser Zelle ab. |
| [DoubleValue](../../aspose.cells.gridweb.data/gridcell/doublevalue) { get; } | Ruft den in der Zelle enthaltenen Double-Wert ab. |
| [FloatValue](../../aspose.cells.gridweb.data/gridcell/floatvalue) { get; } | Ruft den Float-Wert ab, der in der Zelle enthalten ist. |
| [Formula](../../aspose.cells.gridweb.data/gridcell/formula) { get; set; } | Ruft eine Formel von ab oder legt sie festCell . |
| [HtmlString](../../aspose.cells.gridweb.data/gridcell/htmlstring) { get; set; } | Ruft die HTML-Zeichenfolge ab und legt sie fest, die Daten und einige Formatierungen in dieser Zelle enthält. |
| [IntValue](../../aspose.cells.gridweb.data/gridcell/intvalue) { get; } | Ruft den in der Zelle enthaltenen ganzzahligen Wert ab. |
| [IsStyleSet](../../aspose.cells.gridweb.data/gridcell/isstyleset) { get; } | Gibt an, ob der Stil der Zelle eingestellt ist. Wenn "false" zurückgegeben wird, bedeutet dies, dass diese Zelle ein Standardzellenformat hat. |
| [Name](../../aspose.cells.gridweb.data/gridcell/name) { get; } | Ruft den Namen der Zelle ab. Zum Beispiel: A1, F102. |
| [Row](../../aspose.cells.gridweb.data/gridcell/row) { get; } | Ruft die Zeilennummer (nullbasiert) der Zelle ab. |
| [StringValue](../../aspose.cells.gridweb.data/gridcell/stringvalue) { get; } | Ruft den in der Zelle enthaltenen Zeichenfolgenwert ab. |
| [Style](../../aspose.cells.gridweb.data/gridcell/style) { get; set; } | Ruft die Kopie des Zellenstils ab. Legen Sie den Stil für die Zelle fest. |
| [Type](../../aspose.cells.gridweb.data/gridcell/type) { get; } | gibt den Zellwerttyp zurück, die Bedeutung kann GridCellValueType.java entnommen werden |
| [Value](../../aspose.cells.gridweb.data/gridcell/value) { get; set; } | Ruft den in dieser Zelle enthaltenen Wert ab. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [ContainsExternalLink](../../aspose.cells.gridweb.data/gridcell/containsexternallink)() | Gibt an, ob diese Zelle einen externen Link enthält. Gilt nur, wenn die Zelle eine Formelzelle ist. |
| [Copy](../../aspose.cells.gridweb.data/gridcell/copy)(GridCell) | Kopiert Daten aus einer Quellzelle. |
| [CopyStyle](../../aspose.cells.gridweb.data/gridcell/copystyle)(GridTableItemStyle) | kopiere den Stil und setze den Stil für die Zelle |
| [CreateComment](../../aspose.cells.gridweb.data/gridcell/createcomment)(string, string, bool) | Erstellt ein Kommentarobjekt für eine Zelle. |
| [CreateValidation](../../aspose.cells.gridweb.data/gridcell/createvalidation)(GridValidationType, bool) | Erstellt ein Validierungsobjekt für eine Zelle. |
| override [Equals](../../aspose.cells.gridweb.data/gridcell/equals)(object) |  |
| [GetCellArea](../../aspose.cells.gridweb.data/gridcell/getcellarea)() |  |
| [GetComment](../../aspose.cells.gridweb.data/gridcell/getcomment)() | Kommentarobjekt zu dieser Zelle abrufen |
| override [GetHashCode](../../aspose.cells.gridweb.data/gridcell/gethashcode)() |  |
| [GetWidthOfValue](../../aspose.cells.gridweb.data/gridcell/getwidthofvalue)() | Ruft die Breite des Werts in Pixeleinheiten ab. |
| [IsErrorValue](../../aspose.cells.gridweb.data/gridcell/iserrorvalue)() | Prüft, ob eine Formel ein Ergebnis richtig auswerten kann. |
| [IsFormula](../../aspose.cells.gridweb.data/gridcell/isformula)() | Stellt dar, ob die angegebene Zelle eine Formel enthält. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue)(bool) | Fügt einen booleschen Wert in die Zelle ein. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_3)(DateTime) | Fügt einen DateTime-Wert in die Zelle ein. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_1)(double) | Fügt einen doppelten Wert in die Zelle ein. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_2)(int) | Fügt einen int-Wert in die Zelle ein. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_4)(object) | Fügt einen Objektwert in die Zelle ein. Dasselbe wie setValue(Object param_object) |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_5)(string) | Fügt einen String-Wert in die Zelle ein. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_6)(string, bool) | Fügt einen Zeichenfolgenwert in die Zelle ein und konvertiert den Wert gegebenenfalls in einen anderen Datentyp. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_7)(string, bool, bool) | Fügt einen Wert in die Zelle ein, gegebenenfalls wird der Wert in einen anderen Datentyp konvertiert und das Zahlenformat der Zelle wird zurückgesetzt. |
| [PutValueAndSetFormatByValue](../../aspose.cells.gridweb.data/gridcell/putvalueandsetformatbyvalue)(string) | Legt den Wert der Zelle mit einem Zeichenfolgenwert fest und legt das Zellenformat mit diesem Wert fest. |
| [RemoveComment](../../aspose.cells.gridweb.data/gridcell/removecomment)() | Entfernt das Kommentarobjekt der Zelle. |
| [RemoveValidation](../../aspose.cells.gridweb.data/gridcell/removevalidation)() | Entfernt das Validierungsobjekt der Zelle. |
| [SetBorder](../../aspose.cells.gridweb.data/gridcell/setborder)(WebBorderStyle) | Legt Rahmen (oben, unten, links und rechts) für eine Zelle fest, alle Rahmen haben denselben Rahmenstil. |
| [SetCustom](../../aspose.cells.gridweb.data/gridcell/setcustom)(string) | legt das benutzerdefinierte Format fest, null oder leere Zeichenfolge bedeutet kein benutzerdefiniertes Format. |
| [SetFormula](../../aspose.cells.gridweb.data/gridcell/setformula)(string, object) | Stellen Sie die Formel und den Wert der Formel ein. |
| [SetNumberType](../../aspose.cells.gridweb.data/gridcell/setnumbertype)(int) | stellt das Anzeigeformat von Zahlen und Daten ein |
| [ToString](../../aspose.cells.gridweb.data/gridcell/tostring#tostring)() | Gibt eine Zeichenfolge zurück, die das aktuelle Cell-Objekt darstellt. |
| [operator ==](../../aspose.cells.gridweb.data/gridcell/op_equality) |  |
| [operator !=](../../aspose.cells.gridweb.data/gridcell/op_inequality) |  |

### Siehe auch

* namensraum [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data)
* Montage [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
