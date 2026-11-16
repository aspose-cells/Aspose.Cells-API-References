---
title: "GlobalizationSettings Klasse"
linktitle: "GlobalizationSettings"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "GlobalizationSettings class. Kapselt das Objekt, das globalizationsettings in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/globalizationsettings/
---

## GlobalizationSettings class

Stellt die Globalisierungseinstellungen dar.

```go

type GlobalizationSettings struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewGlobalizationSettings](./newglobalizationsettings/) | Standardkonstruktor. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetChartSettings](./getchartsettings/) | Liest die Globalisierungseinstellungen für Diagramm. |
| [SetChartSettings](./setchartsettings/) | Setzt die Globalisierungseinstellungen für Diagramm. |
| [GetPivotSettings](./getpivotsettings/) | Liest die Globalisierungseinstellungen für Pivot-Tabelle. |
| [SetPivotSettings](./setpivotsettings/) | Setzt die Globalisierungseinstellungen für Pivot-Tabelle. |
| [GetTotalName](./gettotalname/) | Liest den Gesamtnamen der Funktion. |
| [GetGrandTotalName](./getgrandtotalname/) | Gibt den Gesamtsummen-Namen der Funktion zurück. |
| [GetDefaultSheetName](./getdefaultsheetname/) | Liest den Standardblattnamen zum automatischen Hinzufügen eines Arbeitsblatts. Standard ist "Sheet". |
| [GetTableRowTypeOfHeaders](./gettablerowtypeofheaders/) | Liest den Typnamen der Tabellenzeilen, die den Tabellenkopf bilden. Standard ist \"Headers\", sodass in der Formel \"#Headers\" den Tabellenkopf repräsentiert. |
| [GetTableRowTypeOfData](./gettablerowtypeofdata/) | Liest den Typnamen der Tabellenzeilen, die den Datenbereich der referenzierten Tabelle bilden. Standard ist \"Data\", sodass in der Formel \"#Data\" den Datenbereich der Tabelle repräsentiert. |
| [GetTableRowTypeOfAll](./gettablerowtypeofall/) | Liest den Typnamen der Tabellenzeilen, die alle Zeilen in der referenzierten Tabelle enthalten. Standard ist "All", sodass in der Formel "#All" alle Zeilen in der referenzierten Tabelle darstellt. |
| [GetTableRowTypeOfTotals](./gettablerowtypeoftotals/) | Liest den Typnamen der Tabellenzeilen, die die Gesamtsumme‑Zeile der referenzierten Tabelle enthalten. Standard ist "Totals", sodass in der Formel "#Totals" die Gesamtsumme‑Zeile der referenzierten Tabelle darstellt. |
| [GetTableRowTypeOfCurrent](./gettablerowtypeofcurrent/) | Liest den Typnamen der Tabellenzeilen, die die aktuelle Zeile in der referenzierten Tabelle enthalten. Standard ist "This Row", sodass in der Formel "#This Row" die aktuelle Zeile in der referenzierten Tabelle darstellt. |
| [GetErrorValueString](./geterrorvaluestring/) | Liest den Anzeigestringwert für den Fehlerwert der Zelle |
| [GetBooleanValueString](./getbooleanvaluestring/) | Liest den Anzeigestringwert für den booleschen Wert der Zelle |
| [GetLocalFunctionName](./getlocalfunctionname/) | Liest den lokalisierungsabhängigen Funktionsnamen gemäß dem angegebenen Standardfunktionsnamen. |
| [GetStandardFunctionName](./getstandardfunctionname/) | Liest den Standardfunktionsnamen gemäß dem angegebenen lokalisierungsabhängigen Funktionsnamen. |
| [GetLocalBuiltInName](./getlocalbuiltinname/) | Liest den lokalisierungsabhängigen Text für den integrierten Namen gemäß dem angegebenen Standardtext. |
| [GetStandardBuiltInName](./getstandardbuiltinname/) | Liest den Standardtext des integrierten Namens gemäß dem angegebenen lokalisierungsabhängigen Text. |
| [GetListSeparator](./getlistseparator/) | Liest das Trennzeichen für Listen, Funktionsparameter, …usw. |
| [GetRowSeparatorOfFormulaArray](./getrowseparatorofformulaarray/) | Liest das Trennzeichen für Zeilen in Array-Daten in Formeln. |
| [GetColumnSeparatorOfFormulaArray](./getcolumnseparatorofformulaarray/) | Liest das Trennzeichen für die Elemente in den Zeilendaten eines Arrays in Formeln. |
| [GetStandardHeaderFooterFontStyleName](./getstandardheaderfooterfontstylename/) | Liest den standardmäßigen englischen Schriftstilnamen (Regular, Bold, Italic) für Kopf-/Fußzeile gemäß dem angegebenen lokalisierungsabhängigen Schriftstilnamen. |
| [GetCommentTitleName](./getcommenttitlename/) | Liest den lokalisierungsabhängigen Kommentar-Titelnamen gemäß dem Kommentar-Titeltyp. |
| [Compare](./compare/) | Vergleicht zwei Zeichenkettenwerte nach bestimmten Sortierregeln. |
