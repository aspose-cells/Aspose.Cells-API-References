---
title: "SettableGlobalizationSettings Klasse"
linktitle: "SettableGlobalizationSettings"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "SettableGlobalizationSettings Klasse. Kapselt das Objekt, das settableglobalizationsettings in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/settableglobalizationsettings/
---

## SettableGlobalizationSettings class

Implementierung von GlobalizationSettings, die dem Benutzer das Festlegen/Ändern vordefinierter Texte ermöglicht.

```go

type SettableGlobalizationSettings struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewSettableGlobalizationSettings](./newsettableglobalizationsettings/) | Standardkonstruktor. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetTotalName](./gettotalname/) | Gibt den Gesamtnamen einer bestimmten Funktion zurück. |
| [SetTotalName](./settotalname/) | Setzt den Gesamtnamen einer bestimmten Funktion. |
| [GetGrandTotalName](./getgrandtotalname/) | Gibt den Gesamtsummen-Namen der Funktion zurück. |
| [SetGrandTotalName](./setgrandtotalname/) | Setzt den Gesamtsummen-Namen einer bestimmten Funktion. |
| [GetTableRowTypeOfHeaders](./gettablerowtypeofheaders/) | Liest den Typnamen der Tabellenzeilen, die den Tabellenkopf bilden. Standard ist \"Headers\", sodass in der Formel \"#Headers\" den Tabellenkopf repräsentiert. |
| [SetTableRowTypeOfHeaders](./settablerowtypeofheaders/) | Setzt den Typnamen der Tabellenzeilen, die den Tabellenkopf bilden. |
| [GetTableRowTypeOfData](./gettablerowtypeofdata/) | Liest den Typnamen der Tabellenzeilen, die den Datenbereich der referenzierten Tabelle bilden. Standard ist \"Data\", sodass in der Formel \"#Data\" den Datenbereich der Tabelle repräsentiert. |
| [SetTableRowTypeOfData](./settablerowtypeofdata/) | Setzt den Typnamen der Tabellenzeilen, die den Datenbereich der referenzierten Tabelle bilden. |
| [GetTableRowTypeOfAll](./gettablerowtypeofall/) | Liest den Typnamen der Tabellenzeilen, die alle Zeilen der referenzierten Tabelle umfassen. |
| [SetTableRowTypeOfAll](./settablerowtypeofall/) | Setzt den Typnamen der Tabellenzeilen, die alle Zeilen der referenzierten Tabelle umfassen. |
| [GetTableRowTypeOfTotals](./gettablerowtypeoftotals/) | Liest den Typnamen der Tabellenzeilen, die die Gesamtsummenzeile der referenzierten Tabelle bilden. |
| [SetTableRowTypeOfTotals](./settablerowtypeoftotals/) | Setzt den Typnamen von Tabellenzeilen, die aus der Gesamtreihe der referenzierten Tabelle bestehen. |
| [GetTableRowTypeOfCurrent](./gettablerowtypeofcurrent/) | Liest den Typnamen von Tabellenzeilen, die aus der aktuellen Zeile in der referenzierten Tabelle bestehen. |
| [SetTableRowTypeOfCurrent](./settablerowtypeofcurrent/) | Setzt den Typnamen von Tabellenzeilen, die aus der aktuellen Zeile in der referenzierten Tabelle bestehen. |
| [GetErrorValueString](./geterrorvaluestring/) | Liest den Anzeigestringwert für den Fehlerwert der Zelle |
| [GetBooleanValueString](./getbooleanvaluestring/) | Liest den Anzeigestringwert für den booleschen Wert der Zelle |
| [SetBooleanValueString](./setbooleanvaluestring/) | Setzt den Anzeigestringwert für den booleschen Wert der Zelle |
| [GetLocalFunctionName](./getlocalfunctionname/) | Liest den lokalisierungsabhängigen Funktionsnamen gemäß dem angegebenen Standardfunktionsnamen. |
| [SetLocalFunctionName](./setlocalfunctionname/) | Setzt den lokalisierungsabhängigen Funktionsnamen, der dem angegebenen Standardfunktionsnamen entspricht. |
| [GetStandardFunctionName](./getstandardfunctionname/) | Liest den Standardfunktionsnamen gemäß dem angegebenen lokalisierungsabhängigen Funktionsnamen. |
| [SetStandardFunctionName](./setstandardfunctionname/) | Setzt den lokalisierungsabhängigen Funktionsnamen gemäß dem angegebenen Standardfunktionsnamen. |
| [GetLocalBuiltInName](./getlocalbuiltinname/) | Liest den lokalisierungsabhängigen Text für den integrierten Namen gemäß dem angegebenen Standardtext. |
| [SetLocalBuiltInName](./setlocalbuiltinname/) | Setzt den lokalisierungsabhängigen Text für den integrierten Namen mit dem angegebenen Standardnamen-Text. |
| [GetStandardBuiltInName](./getstandardbuiltinname/) | Liest den Standardtext des integrierten Namens gemäß dem angegebenen lokalisierungsabhängigen Text. |
| [SetStandardBuiltInName](./setstandardbuiltinname/) | Setzt den lokalisierungsabhängigen Funktionsnamen gemäß dem angegebenen Standardfunktionsnamen. |
| [GetListSeparator](./getlistseparator/) | Liest das Trennzeichen für Listen, Funktionsparameter, …usw. |
| [SetListSeparator](./setlistseparator/) | Setzt das Trennzeichen für Listen, Funktionsparameter, …usw. |
| [GetRowSeparatorOfFormulaArray](./getrowseparatorofformulaarray/) | Liest das Trennzeichen für Zeilen in Array-Daten in Formeln. |
| [SetRowSeparatorOfFormulaArray](./setrowseparatorofformulaarray/) | Setzt das Trennzeichen für Zeilen in Array-Daten in Formeln. |
| [GetColumnSeparatorOfFormulaArray](./getcolumnseparatorofformulaarray/) | Liest das Trennzeichen für die Elemente in den Zeilendaten eines Arrays in Formeln. |
| [SetColumnSeparatorOfFormulaArray](./setcolumnseparatorofformulaarray/) | Setzt das Trennzeichen für die Elemente in den Zeilendaten eines Arrays in Formeln. |
| [GetStandardHeaderFooterFontStyleName](./getstandardheaderfooterfontstylename/) | Liest den standardmäßigen englischen Schriftstilnamen (Regular, Bold, Italic) für Kopf-/Fußzeile gemäß dem angegebenen lokalisierungsabhängigen Schriftstilnamen. |
| [SetStandardHeaderFooterFontStyleName](./setstandardheaderfooterfontstylename/) | Setzt den lokalisierungsabhängigen Funktionsnamen gemäß dem angegebenen Standardfunktionsnamen. |
| [GetCommentTitleName](./getcommenttitlename/) | Liest den lokalisierungsabhängigen Kommentar-Titelnamen gemäß dem Kommentar-Titeltyp. |
| [SetCommentTitleName](./setcommenttitlename/) | Liest den lokalisierungsabhängigen Kommentar-Titelnamen gemäß dem Kommentar-Titeltyp. |
