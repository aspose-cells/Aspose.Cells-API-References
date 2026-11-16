---
title: "DbfLoadOptions-Klasse"
linktitle: "DbfLoadOptions"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "DbfLoadOptions-Klasse. Kapselt das Objekt, das dbfloadoptions in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/dbfloadoptions/
---

## DbfLoadOptions class

Stellt die Optionen zum Laden einer .dbf-Datei dar.

```go

type DbfLoadOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewDbfLoadOptions](./newdbfloadoptions/) | Die Optionen. |
| [NewDbfLoadOptions_LoadOptions](./newdbfloadoptions_loadoptions/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
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
