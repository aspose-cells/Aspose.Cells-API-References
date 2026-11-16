---
title: "TxtLoadOptions Klasse"
linktitle: "TxtLoadOptions"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "TxtLoadOptions Klasse. Kapselt das Objekt, das txtloadoptions in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/txtloadoptions/
---

## TxtLoadOptions class

Stellt die Optionen zum Laden einer Textdatei dar.

```go

type TxtLoadOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewTxtLoadOptions](./newtxtloadoptions/) | Erstellt die Optionen zum Laden einer Textdatei. |
| [NewTxtLoadOptions_LoadFormat](./newtxtloadoptions_loadformat/) | Erstellt die Optionen zum Laden einer Textdatei. |
| [NewTxtLoadOptions_AbstractTextLoadOptions](./newtxtloadoptions_abstracttextloadoptions/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetSeparator](./getseparator/) | Liest und setzt das Zeichen-Trennzeichen der Textdatei. |
| [SetSeparator](./setseparator/) | Liest und setzt das Zeichen-Trennzeichen der Textdatei. |
| [GetSeparatorString](./getseparatorstring/) | Liest und setzt einen Zeichenkettenwert als Trennzeichen. |
| [SetSeparatorString](./setseparatorstring/) | Liest und setzt einen Zeichenkettenwert als Trennzeichen. |
| [IsMultiEncoded](./ismultiencoded/) | True bedeutet, dass die Datei mehrere Codierungen enthält. |
| [SetIsMultiEncoded](./setismultiencoded/) | True bedeutet, dass die Datei mehrere Codierungen enthält. |
| [GetHasFormula](./gethasformula/) | Gibt an, ob der Text eine Formel ist, wenn er mit "=" beginnt. |
| [SetHasFormula](./sethasformula/) | Gibt an, ob der Text eine Formel ist, wenn er mit "=" beginnt. |
| [GetHasTextQualifier](./gethastextqualifier/) | Gibt an, ob ein Textqualifizierer für den Zellenwert vorhanden ist. Standard ist true. |
| [SetHasTextQualifier](./sethastextqualifier/) | Gibt an, ob ein Textqualifizierer für den Zellenwert vorhanden ist. Standard ist true. |
| [GetTextQualifier](./gettextqualifier/) | Gibt den Textqualifizierer für Zellenwerte an. Standardqualifizierer ist '"'. |
| [SetTextQualifier](./settextqualifier/) | Gibt den Textqualifizierer für Zellenwerte an. Standardqualifizierer ist '"'. |
| [GetTreatConsecutiveDelimitersAsOne](./gettreatconsecutivedelimitersasone/) | Gibt an, ob aufeinanderfolgende Trennzeichen als eines behandelt werden sollen. |
| [SetTreatConsecutiveDelimitersAsOne](./settreatconsecutivedelimitersasone/) | Gibt an, ob aufeinanderfolgende Trennzeichen als eines behandelt werden sollen. |
| [GetTreatQuotePrefixAsValue](./gettreatquoteprefixasvalue/) | Gibt an, ob das führende einfache Anführungszeichen als Teil des Werts einer Zelle betrachtet werden soll. Standard ist true. Wenn es false ist, wird das führende einfache Anführungszeichen aus dem entsprechenden Zellenwert entfernt und Style.QuotePrefix wird für die Zelle auf true gesetzt. |
| [SetTreatQuotePrefixAsValue](./settreatquoteprefixasvalue/) | Gibt an, ob das führende einfache Anführungszeichen als Teil des Werts einer Zelle betrachtet werden soll. Standard ist true. Wenn es false ist, wird das führende einfache Anführungszeichen aus dem entsprechenden Zellenwert entfernt und Style.QuotePrefix wird für die Zelle auf true gesetzt. |
| [GetExtendToNextSheet](./getextendtonextsheet/) | Gibt an, ob Daten auf das nächste Blatt erweitert werden, wenn die Zeilen- oder Spaltenanzahl das Limit überschreitet. Standard ist false. |
| [SetExtendToNextSheet](./setextendtonextsheet/) | Gibt an, ob Daten auf das nächste Blatt erweitert werden, wenn die Zeilen- oder Spaltenanzahl das Limit überschreitet. Standard ist false. |
| [GetHeaderRowsCount](./getheaderrowscount/) | Die Anzahl der Kopfzeilen, die für erweiterte Blätter wiederholt werden. |
| [SetHeaderRowsCount](./setheaderrowscount/) | Die Anzahl der Kopfzeilen, die für erweiterte Blätter wiederholt werden. |
| [GetHeaderColumnsCount](./getheadercolumnscount/) | Die Anzahl der Kopfspalten, die für erweiterte Blätter wiederholt werden. |
| [SetHeaderColumnsCount](./setheadercolumnscount/) | Die Anzahl der Kopfspalten, die für erweiterte Blätter wiederholt werden. |
| [GetMaxRowCount](./getmaxrowcount/) | Die maximale Anzahl von Zeilen, die für ein Blatt importiert werden können. |
| [SetMaxRowCount](./setmaxrowcount/) | Die maximale Anzahl von Zeilen, die für ein Blatt importiert werden können. |
| [GetMaxColumnCount](./getmaxcolumncount/) | Die maximale Anzahl von Spalten, die für ein Blatt importiert werden können. |
| [SetMaxColumnCount](./setmaxcolumncount/) | Die maximale Anzahl von Spalten, die für ein Blatt importiert werden können. |
| [GetEncoding](./getencoding/) | Liest und setzt die Standardkodierung. Gilt nur für CSV-Dateien. |
| [SetEncoding](./setencoding/) | Liest und setzt die Standardkodierung. Gilt nur für CSV-Dateien. |
| [GetLoadStyleStrategy](./getloadstylestrategy/) | Gibt die Strategie an, mit der Stil für geparste Werte angewendet wird, wenn ein Zeichenkettenwert in eine Zahl oder ein Datum/Uhrzeit konvertiert wird. |
| [SetLoadStyleStrategy](./setloadstylestrategy/) | Gibt die Strategie an, mit der Stil für geparste Werte angewendet wird, wenn ein Zeichenkettenwert in eine Zahl oder ein Datum/Uhrzeit konvertiert wird. |
| [GetConvertNumericData](./getconvertnumericdata/) | Liest oder setzt einen Wert, der angibt, ob die Zeichenkette in einer Textdatei in numerische Daten konvertiert wird.Standardwert ist wahr. |
| [SetConvertNumericData](./setconvertnumericdata/) | Liest oder setzt einen Wert, der angibt, ob die Zeichenkette in einer Textdatei in numerische Daten konvertiert wird.Standardwert ist wahr. |
| [GetConvertDateTimeData](./getconvertdatetimedata/) | Liest oder setzt einen Wert, der angibt, ob die Zeichenkette in einer Textdatei in Datumsdaten konvertiert wird.Standardwert ist wahr. |
| [SetConvertDateTimeData](./setconvertdatetimedata/) | Liest oder setzt einen Wert, der angibt, ob die Zeichenkette in einer Textdatei in Datumsdaten konvertiert wird.Standardwert ist wahr. |
| [GetKeepPrecision](./getkeepprecision/) | Gibt an, ob ein Zeichenkettenwert bei einer Länge von 15 nicht geparst wird. |
| [SetKeepPrecision](./setkeepprecision/) | Gibt an, ob ein Zeichenkettenwert bei einer Länge von 15 nicht geparst wird. |
| [GetLoadFormat](./getloadformat/) | Liest das Ladeformat. |
| [GetPassword](./getpassword/) | Liest und setzt das Passwort der Arbeitsmappe. |
| [SetPassword](./setpassword/) | Liest und setzt das Passwort der Arbeitsmappe. |
| [GetParsingFormulaOnOpen](./getparsingformulaonopen/) | Gibt an, ob die Formel beim Lesen der Datei geparst wird. |
| [SetParsingFormulaOnOpen](./setparsingformulaonopen/) | Gibt an, ob die Formel beim Lesen der Datei geparst wird. |
| [GetParsingPivotCachedRecords](./getparsingpivotcachedrecords/) | Gibt an, ob zwischengespeicherte Pivot‑Datensätze beim Laden der Datei geparst werden.Standardwert ist falsch. |
| [SetParsingPivotCachedRecords](./setparsingpivotcachedrecords/) | Gibt an, ob zwischengespeicherte Pivot‑Datensätze beim Laden der Datei geparst werden.Standardwert ist falsch. |
| [SetPaperSize](./setpapersize/) | Setzt die Standard-Papiergröße für den Druck aus den Einstellungen des Standarddruckers. |
| [GetLanguageCode](./getlanguagecode/) | Liest oder setzt die Sprache der Benutzeroberfläche der Arbeitsmappen‑Version basierend auf dem Ländercode, in dem die Datei gespeichert wurde. |
| [SetLanguageCode](./setlanguagecode/) | Liest oder setzt die Sprache der Benutzeroberfläche der Arbeitsmappen‑Version basierend auf dem Ländercode, in dem die Datei gespeichert wurde. |
| [GetRegion](./getregion/) | Liest oder setzt die regionalen Einstellungen, die für die zu ladende Arbeitsmappe verwendet werden. |
| [SetRegion](./setregion/) | Liest oder setzt die regionalen Einstellungen, die für die zu ladende Arbeitsmappe verwendet werden. |
| [GetDefaultStyleSettings](./getdefaultstylesettings/) | Liest die Standardstil‑Einstellungen zum Initialisieren von Stilen der Arbeitsmappe |
| [GetInterruptMonitor](./getinterruptmonitor/) | Liest und setzt den Interrupt‑Monitor. |
| [SetInterruptMonitor](./setinterruptmonitor/) | Liest und setzt den Interrupt‑Monitor. |
| [GetIgnoreNotPrinted](./getignorenotprinted/) | Ignoriere die Daten, die nicht gedruckt werden, wenn die Datei direkt gedruckt wird |
| [SetIgnoreNotPrinted](./setignorenotprinted/) | Ignoriere die Daten, die nicht gedruckt werden, wenn die Datei direkt gedruckt wird |
| [GetCheckDataValid](./getcheckdatavalid/) | Prüfe, ob die Daten in der Vorlagendatei gültig sind. |
| [SetCheckDataValid](./setcheckdatavalid/) | Prüfe, ob die Daten in der Vorlagendatei gültig sind. |
| [GetCheckExcelRestriction](./getcheckexcelrestriction/) | Ob die Beschränkungen einer Excel‑Datei geprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Zum Beispiel erlaubt Excel nicht, einen Zeichenkettenwert länger als 32 K einzugeben. Wenn Sie einen Wert länger als 32 K, etwa mit Cell.PutValue(string), eingeben, erhalten Sie bei true‑Eigenschaft eine Ausnahme. Ist die Eigenschaft false, akzeptieren wir Ihren Eingabe‑Zeichenkettenwert als Zellwert, sodass Sie später den vollständigen Zeichenkettenwert für andere Dateiformate wie CSV ausgeben können. Wenn Sie jedoch einen Wert festlegen, der für das Excel‑Dateiformat ungültig ist, sollten Sie die Arbeitsmappe später nicht im Excel‑Format speichern. Andernfalls kann es zu unerwarteten Fehlern in der erzeugten Excel‑Datei kommen. |
| [SetCheckExcelRestriction](./setcheckexcelrestriction/) | Ob die Beschränkungen einer Excel‑Datei geprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Zum Beispiel erlaubt Excel nicht, einen Zeichenkettenwert länger als 32 K einzugeben. Wenn Sie einen Wert länger als 32 K, etwa mit Cell.PutValue(string), eingeben, erhalten Sie bei true‑Eigenschaft eine Ausnahme. Ist die Eigenschaft false, akzeptieren wir Ihren Eingabe‑Zeichenkettenwert als Zellwert, sodass Sie später den vollständigen Zeichenkettenwert für andere Dateiformate wie CSV ausgeben können. Wenn Sie jedoch einen Wert festlegen, der für das Excel‑Dateiformat ungültig ist, sollten Sie die Arbeitsmappe später nicht im Excel‑Format speichern. Andernfalls kann es zu unerwarteten Fehlern in der erzeugten Excel‑Datei kommen. |
| [GetKeepUnparsedData](./getkeepunparseddata/) | Ob die nicht geparsten Daten im Speicher für die Arbeitsmappe gehalten werden, wenn sie aus einer Vorlagendatei geladen wird. Standard ist wahr. |
| [SetKeepUnparsedData](./setkeepunparseddata/) | Ob die nicht geparsten Daten im Speicher für die Arbeitsmappe gehalten werden, wenn sie aus einer Vorlagendatei geladen wird. Standard ist wahr. |
| [GetLoadFilter](./getloadfilter/) | Der Filter, der angibt, wie Daten geladen werden. |
| [SetLoadFilter](./setloadfilter/) | Der Filter, der angibt, wie Daten geladen werden. |
| [GetMemorySetting](./getmemorysetting/) | Liest oder setzt den Speichermodus für geladene Arbeitsmappen. |
| [SetMemorySetting](./setmemorysetting/) | Liest oder setzt den Speichermodus für geladene Arbeitsmappen. |
| [GetAutoFitterOptions](./getautofitteroptions/) | Liest und setzt die Auto‑Fit‑Optionen |
| [SetAutoFitterOptions](./setautofitteroptions/) | Liest und setzt die Auto‑Fit‑Optionen |
| [GetAutoFilter](./getautofilter/) | Gibt an, ob die Daten beim Laden der Dateien automatisch gefiltert werden. |
| [SetAutoFilter](./setautofilter/) | Gibt an, ob die Daten beim Laden der Dateien automatisch gefiltert werden. |
| [GetFontConfigs](./getfontconfigs/) | Liest und setzt einzelne Schriftart‑Konfigurationen. Funktioniert nur für die Arbeitsmappe, die diese LoadOptions zum Laden verwendet. |
| [SetFontConfigs](./setfontconfigs/) | Liest und setzt einzelne Schriftart‑Konfigurationen. Funktioniert nur für die Arbeitsmappe, die diese LoadOptions zum Laden verwendet. |
| [GetIgnoreUselessShapes](./getignoreuselessshapes/) | Gibt an, ob nutzlose Formen ignoriert werden. |
| [SetIgnoreUselessShapes](./setignoreuselessshapes/) | Gibt an, ob nutzlose Formen ignoriert werden. |
| [GetPreservePaddingSpacesInFormula](./getpreservepaddingspacesinformula/) | Gibt an, ob die Leerzeichen und Zeilenumbrüche, die zwischen Formeltoken eingefügt werden, beim Lesen und Schreiben von Formeln beibehalten werden. Standardwert ist false. |
| [SetPreservePaddingSpacesInFormula](./setpreservepaddingspacesinformula/) | Gibt an, ob die Leerzeichen und Zeilenumbrüche, die zwischen Formeltoken eingefügt werden, beim Lesen und Schreiben von Formeln beibehalten werden. Standardwert ist false. |
