---
title: "Zellenklasse"
linktitle: "Zelle"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "Zellenklasse. Kapselt das Objekt, das Zelle in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/cell/
---

## Cell class

Kapselt das Objekt, das eine einzelne Arbeitsmappen‑Zelle darstellt.

```go

type Cell struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [Calculate](./calculate/) | Berechnet die Formel der Zelle. |
| [GetWorksheet](./getworksheet/) | Liefert das übergeordnete Arbeitsblatt. |
| [PutValue_Bool](./putvalue_bool/) | Setzt einen booleschen Wert in die Zelle. |
| [PutValue_Int](./putvalue_int/) | Setzt einen ganzzahligen Wert in die Zelle. |
| [PutValue_Double](./putvalue_double/) | Setzt einen Gleitkommawert in die Zelle. |
| [PutValue_String_Bool_Bool](./putvalue_string_bool_bool/) | Setzt einen Wert in die Zelle, falls zutreffend wird der Wert in einen anderen Datentyp konvertiert und das Zahlenformat der Zelle wird zurückgesetzt. |
| [PutValue_String_Bool](./putvalue_string_bool/) | Setzt einen Zeichenkettenwert in die Zelle und konvertiert den Wert, falls zutreffend, in einen anderen Datentyp. |
| [PutValue_String](./putvalue_string/) | Setzt einen Zeichenkettenwert in die Zelle. |
| [PutValue_Date](./putvalue_date/) | Setzt einen DateTime-Wert in die Zelle. |
| [PutValue_Object](./putvalue_object/) | Setzt einen Objektwert in die Zelle. |
| [GetRow](./getrow/) | Liefert die Zeilennummer (nullbasiert) der Zelle. |
| [GetColumn](./getcolumn/) | Liefert die Spaltennummer (nullbasiert) der Zelle. |
| [IsFormula](./isformula/) | Gibt an, ob die angegebene Zelle eine Formel enthält. |
| [GetHasCustomFunction](./gethascustomfunction/) | Prüft, ob in der Formel dieser Zelle eine benutzerdefinierte Funktion (nicht unterstützte Funktion) vorhanden ist. |
| [GetType](./gettype/) | Stellt den Zellenwerttyp dar. |
| [GetName](./getname/) | Liefert den Namen der Zelle. |
| [IsErrorValue](./iserrorvalue/) | Prüft, ob der Wert dieser Zelle ein Fehler ist. |
| [IsNumericValue](./isnumericvalue/) | Gibt an, ob der Wert dieser Zelle numerisch ist (int, double und datetime). |
| [GetStringValue_CellValueFormatStrategy](./getstringvalue_cellvalueformatstrategy/) | Liefert den Zeichenkettenwert nach einer spezifischen Formatierungsstrategie. |
| [GetStringValue](./getstringvalue/) | Liefert den in der Zelle enthaltenen Zeichenkettenwert. Wenn der Typ dieser Zelle Zeichenkette ist, wird der Zeichenkettenwert selbst zurückgegeben. Für andere Zellentypen wird der formatierte Zeichenkettenwert (formatiert mit dem angegebenen Stil dieser Zelle) zurückgegeben. Der formatierte Zellenwert entspricht dem, was Sie in Excel erhalten, wenn Sie eine Zelle als Text kopieren (z. B. das Kopieren der Zelle in einen Texteditor oder das Exportieren in CSV). |
| [GetNumberCategoryType](./getnumbercategorytype/) | Stellt den Kategorie‑Typ der Zahlenformatierung dieser Zelle dar. |
| [GetDisplayStringValue](./getdisplaystringvalue/) | Ermittelt den formatierten Zeichenkettenwert dieser Zelle gemäß dem Anzeigeformat der Zelle. |
| [GetIntValue](./getintvalue/) | Ermittelt den ganzzahligen Wert, der in der Zelle enthalten ist. |
| [GetDoubleValue](./getdoublevalue/) | Ermittelt den double‑Wert, der in der Zelle enthalten ist. |
| [GetFloatValue](./getfloatvalue/) | Ermittelt den float‑Wert, der in der Zelle enthalten ist. |
| [GetDateTimeValue](./getdatetimevalue/) | Ermittelt den DateTime‑Wert, der in der Zelle enthalten ist. |
| [GetBoolValue](./getboolvalue/) | Ermittelt den booleschen Wert, der in der Zelle enthalten ist. |
| [GetWidthOfValue](./getwidthofvalue/) | Ermittelt die Breite des Werts in Pixeln. |
| [GetHeightOfValue](./getheightofvalue/) | Ermittelt die Höhe des Werts in Pixeln. |
| [GetDisplayStyle](./getdisplaystyle/) | Ermittelt das Anzeigeformat dieser Zelle. |
| [GetDisplayStyle_Bool](./getdisplaystyle_bool/) | Ermittelt das Anzeigeformat dieser Zelle. |
| [GetDisplayStyle_BorderType](./getdisplaystyle_bordertype/) | Ermittelt das Anzeigeformat dieser Zelle. |
| [GetFormatConditions](./getformatconditions/) | Ermittelt die Formatbedingungen, die auf diese Zelle angewendet werden. |
| [GetStyle](./getstyle/) | Ermittelt den Zellenstil. |
| [GetStyle_Bool](./getstyle_bool/) | Wenn checkBorders true ist, prüfen, ob die Ränder anderer Zellen den Stil dieser Zelle beeinflussen. |
| [SetStyle_Style](./setstyle_style/) | Setzt den Zellenstil. |
| [SetStyle_Style_Bool](./setstyle_style_bool/) | Wendet die geänderten Stileigenschaften auf die Zelle an. |
| [SetStyle_Style_StyleFlag](./setstyle_style_styleflag/) | Wendet den Zellenstil basierend auf Flags an. |
| [GetHasCustomStyle](./gethascustomstyle/) | Gibt an, ob diese Zelle benutzerdefinierte Stileinstellungen hat (anders als die standardmäßige, die von der entsprechenden Zeile, Spalte oder Arbeitsmappe geerbt wird). |
| [GetSharedStyleIndex](./getsharedstyleindex/) | Ermittelt den gemeinsamen Stilindex der Zelle im Stilpool. |
| [GetFormula](./getformula/) | Ermittelt oder setzt eine Formel der Zelle. |
| [SetFormula_String](./setformula_string/) | Ermittelt oder setzt eine Formel der Zelle. |
| [GetFormulaLocal](./getformulalocal/) | Ermittelt die lokalisierte formatierte Formel der Zelle. |
| [SetFormulaLocal](./setformulalocal/) | Ermittelt die lokalisierte formatierte Formel der Zelle. |
| [GetR1C1Formula](./getr1c1formula/) | Ermittelt oder setzt eine R1C1‑Formel der Zelle. |
| [SetR1C1Formula](./setr1c1formula/) | Ermittelt oder setzt eine R1C1‑Formel der Zelle. |
| [SetFormula_String_Object](./setformula_string_object/) | Setzt die Formel und den Wert (berechnetes Ergebnis) der Formel. |
| [SetFormula_String_FormulaParseOptions](./setformula_string_formulaparseoptions/) | Setzt die Formel und den Wert (berechnetes Ergebnis) der Formel. |
| [GetFormula_Bool_Bool](./getformula_bool_bool/) | Ermittelt die Formel dieser Zelle. |
| [SetFormula_String_FormulaParseOptions_Object](./setformula_string_formulaparseoptions_object/) | Setzt die Formel und den Wert (berechnetes Ergebnis) der Formel. |
| [SetArrayFormula_String_Int_Int](./setarrayformula_string_int_int/) | Setzt eine Array‑Formel (Legacy‑Array‑Formel, die über STRG+UMSCHALT+EINGABE in MS Excel eingegeben wird) für einen Zellbereich. |
| [SetArrayFormula_String_Int_Int_FormulaParseOptions](./setarrayformula_string_int_int_formulaparseoptions/) | Setzt eine Array‑Formel für einen Zellbereich. |
| [SetArrayFormula_String_Int_Int_FormulaParseOptions_Object2Array](./setarrayformula_string_int_int_formulaparseoptions_object2array/) | Setzt eine Array‑Formel für einen Zellbereich. |
| [SetSharedFormula_String_Int_Int](./setsharedformula_string_int_int/) | Legt gemeinsam genutzte Formeln für einen Zellbereich fest. |
| [SetSharedFormula_String_Int_Int_FormulaParseOptions](./setsharedformula_string_int_int_formulaparseoptions/) | Legt gemeinsam genutzte Formeln für einen Zellbereich fest. |
| [SetSharedFormula_String_Int_Int_FormulaParseOptions_Object2Array](./setsharedformula_string_int_int_formulaparseoptions_object2array/) | Legt gemeinsam genutzte Formeln für einen Zellbereich fest. |
| [GetContainsExternalLink](./getcontainsexternallink/) | Gibt an, ob diese Zelle einen externen Link enthält. Gilt nur, wenn die Zelle eine Formelzelle ist. |
| [GetPrecedents](./getprecedents/) | Liefert alle Verweise, die in der Formel dieser Zelle vorkommen. |
| [GetDependents](./getdependents/) | Ermittelt alle Zellen, deren Formel direkt auf diese Zelle verweist. |
| [GetPrecedentsInCalculation](./getprecedentsincalculation/) | Liefert alle Vorgänger (Verweise auf Zellen in der aktuellen Arbeitsmappe), die von der Formel dieser Zelle bei der Berechnung verwendet werden. |
| [GetDependentsInCalculation](./getdependentsincalculation/) | Liefert alle Zellen, deren berechnetes Ergebnis von dieser Zelle abhängt. |
| [IsArrayHeader](./isarrayheader/) | Gibt an, dass die Formel der Zelle eine Array-Formel ist und dass sie die erste Zelle des Arrays ist. |
| [IsDynamicArrayFormula](./isdynamicarrayformula/) | Gibt an, ob die Formel der Zelle eine dynamische Array-Formel (true) oder eine klassische Array-Formel (false) ist. |
| [GetArrayRange](./getarrayrange/) | Liefert den Array‑Bereich, wenn die Formel der Zelle eine Array-Formel ist. |
| [IsArrayFormula](./isarrayformula/) | Gibt an, ob die Zellformel eine Array-Formel ist. |
| [IsSharedFormula](./issharedformula/) | Gibt an, ob die Zellformel Teil einer gemeinsam genutzten Formel ist. |
| [IsTableFormula](./istableformula/) | Gibt an, ob diese Zelle Teil einer Tabellenformel ist. |
| [SetDynamicArrayFormula_String_FormulaParseOptions_Bool](./setdynamicarrayformula_string_formulaparseoptions_bool/) | Legt eine dynamische Array-Formel fest und lässt die Formel, falls möglich, in benachbarte Zellen überlaufen. |
| [SetDynamicArrayFormula_String_FormulaParseOptions_Object2Array_Bool_Bool](./setdynamicarrayformula_string_formulaparseoptions_object2array_bool_bool/) | Legt eine dynamische Array-Formel fest und lässt die Formel, falls möglich, in benachbarte Zellen überlaufen. |
| [SetDynamicArrayFormula_String_FormulaParseOptions_Object2Array_Bool_Bool_CalculationOptions](./setdynamicarrayformula_string_formulaparseoptions_object2array_bool_bool_calculationoptions/) | Legt eine dynamische Array-Formel fest und lässt die Formel, falls möglich, in benachbarte Zellen überlaufen. |
| [SetTableFormula_Int_Int_String_String_Object2Array](./settableformula_int_int_string_string_object2array/) | Erstellt eine zweidimensionale Datentabelle für den angegebenen Bereich, beginnend mit dieser Zelle. |
| [SetTableFormula_Int_Int_String_Bool_Object2Array](./settableformula_int_int_string_bool_object2array/) | Erstellt eine eindimensionale Datentabelle für den angegebenen Bereich, beginnend mit dieser Zelle. |
| [SetTableFormula_Int_Int_Int_Int_Int_Int_Object2Array](./settableformula_int_int_int_int_int_int_object2array/) | Erstellt eine zweidimensionale Datentabelle für den angegebenen Bereich, beginnend mit dieser Zelle. |
| [SetTableFormula_Int_Int_Int_Int_Bool_Object2Array](./settableformula_int_int_int_int_bool_object2array/) | Erstellt eine eindimensionale Datentabelle für den angegebenen Bereich, beginnend mit dieser Zelle. |
| [RemoveArrayFormula](./removearrayformula/) | Array-Formel entfernen. |
| [Copy](./copy/) | Kopiert Daten aus einer Quellzelle. |
| [GetValue](./getvalue/) | Liefert/setzt den in dieser Zelle enthaltenen Wert. |
| [SetValue](./setvalue/) | Liefert/setzt den in dieser Zelle enthaltenen Wert. |
| [IsStyleSet](./isstyleset/) | Gibt an, ob der Zellenstil festgelegt ist. Wenn false zurückgegeben wird, bedeutet dies, dass diese Zelle das Standardzellenformat hat. |
| [Characters](./characters/) | Gibt ein Characters-Objekt zurück, das einen Zeichenbereich im Zelltext darstellt. |
| [Replace](./replace/) | Ersetzt den Text der Zelle mit Optionen. |
| [InsertText](./inserttext/) | Fügt der Zelle einige Zeichen hinzu. Wenn die Zelle reich formatiert ist, kann diese Methode die ursprüngliche Formatierung beibehalten. |
| [IsRichText](./isrichtext/) | Gibt an, ob der Zeichenkettenwert dieser Zelle ein reich formatierter Text ist. |
| [GetCharacters](./getcharacters/) | Gibt alle Characters-Objekte zurück, die einen Zeichenbereich im Zelltext darstellen. |
| [GetCharacters_Bool](./getcharacters_bool/) | Gibt alle Characters-Objekte zurück, die einen Zeichenbereich im Zelltext darstellen. |
| [SetCharacters](./setcharacters/) | Legt das Rich-Text-Format der Zelle fest. |
| [IsMerged](./ismerged/) | Prüft, ob eine Zelle Teil eines zusammengeführten Bereichs ist oder nicht. |
| [GetMergedRange](./getmergedrange/) | Gibt ein Range-Objekt zurück, das einen zusammengeführten Bereich darstellt. |
| [GetComment](./getcomment/) | Liefert den Kommentar dieser Zelle. |
| [GetHtmlString](./gethtmlstring/) | Liest und schreibt die HTML-Zeichenkette, die Daten und einige Formate in dieser Zelle enthält. |
| [SetHtmlString](./sethtmlstring/) | Liest und schreibt die HTML-Zeichenkette, die Daten und einige Formate in dieser Zelle enthält. |
| [GetHtmlString_Bool](./gethtmlstring_bool/) | Liest die HTML-Zeichenkette, die Daten und einige Formate in dieser Zelle enthält. |
| [ToString](./tostring/) | Gibt einen String zurück, der das aktuelle Cell‑Objekt darstellt. |
| [ToJson](./tojson/) | Konvertiert eine Zelle in JSON-Strukturdaten. |
| [Equals_Object](./equals_object/) | Prüft, ob dieses Objekt auf dieselbe Zelle wie ein anderes verweist. |
| [GetHashCode](./gethashcode/) | Dient als Hash-Funktion für einen bestimmten Typ. |
| [Equals_Cell](./equals_cell/) | Prüft, ob dieses Objekt auf dieselbe Zelle wie ein anderes Zellenobjekt verweist. |
| [GetConditionalFormattingResult](./getconditionalformattingresult/) | Ermittelt das Ergebnis der bedingten Formatierung. |
| [GetValidation](./getvalidation/) | Liefert die auf diese Zelle angewendete Validierung. |
| [GetValidationValue](./getvalidationvalue/) | Liefert den Wert der Validierung, die auf diese Zelle angewendet wurde. |
| [GetTable](./gettable/) | Liefert die Tabelle, die diese Zelle enthält. |
| [IsCheckBoxStyle](./ischeckboxstyle/) | Gibt an, ob diese Zelle als Kontrollkästchen festgelegt ist. |
| [SetIsCheckBoxStyle](./setischeckboxstyle/) | Gibt an, ob diese Zelle als Kontrollkästchen festgelegt ist. |
| [GetRichValue](./getrichvalue/) | Liefert den Rich-Wert der Zelle. |
| [GetEmbeddedImage](./getembeddedimage/) | Liest und schreibt das eingebettete Bild in der Zelle. |
| [SetEmbeddedImage](./setembeddedimage/) | Liest und schreibt das eingebettete Bild in der Zelle. |
| [GetPicture](./getpicture/) | Liefert eine Aspose.Cells.Drawing.Picture-Instanz, die das eingebettete Bild in dieser Zelle darstellt, oder null, wenn für diese Zelle kein eingebettetes Bild vorhanden ist. |
|[Dispose](./dispose/) |  | 
