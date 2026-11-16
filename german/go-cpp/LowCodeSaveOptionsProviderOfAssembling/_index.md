---
title: "LowCodeSaveOptionsProviderOfAssembling Klasse"
linktitle: "LowCodeSaveOptionsProviderOfAssembling"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "LowCodeSaveOptionsProviderOfAssembling-Klasse. Kapselt das Objekt, das lowcodesaveoptionsproviderofassembling in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/lowcodesaveoptionsproviderofassembling/
---

## LowCodeSaveOptionsProviderOfAssembling class

Implementierung zur Bereitstellung von Speicheroptionen, die geteilte Teile in Dateien speichern und deren Pfad wie folgt benannt wird (kann Verzeichnisse enthalten): <see cref="PathHeader"/>+<see cref="SheetPrefix"/>+SheetIndex(oder SheetName)+<see cref="SplitPartPrefix"/>+SplitPartIndex+<see cref="PathTail"/>.

```go

type LowCodeSaveOptionsProviderOfAssembling struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewLowCodeSaveOptionsProviderOfAssembling](./newlowcodesaveoptionsproviderofassembling/) | Standardkonstruktor. |
| [NewLowCodeSaveOptionsProviderOfAssembling_AbstractLowCodeSaveOptionsProvider](./newlowcodesaveoptionsproviderofassembling_abstractlowcodesaveoptionsprovider/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetPathHeader](./getpathheader/) | Kopfteil (vor hinzugefügtem Inhalt des Blatts und des geteilten Teils) des Dateipfads. |
| [SetPathHeader](./setpathheader/) | Kopfteil (vor hinzugefügtem Inhalt des Blatts und des geteilten Teils) des Dateipfads. |
| [GetPathTail](./getpathtail/) | Endteil (nach Sequenznummern) des Dateipfads. Er sollte die Dateinamenerweiterung enthalten. |
| [SetPathTail](./setpathtail/) | Endteil (nach Sequenznummern) des Dateipfads. Er sollte die Dateinamenerweiterung enthalten. |
| [GetUseSheetName](./getusesheetname/) | Ob der Dateipfad mit Blattnamen anstelle des Blattindexes erstellt wird. Standardwert ist false. |
| [SetUseSheetName](./setusesheetname/) | Ob der Dateipfad mit Blattnamen anstelle des Blattindexes erstellt wird. Standardwert ist false. |
| [GetSheetPrefix](./getsheetprefix/) | Präfix für den Index des Arbeitsblatts. |
| [SetSheetPrefix](./setsheetprefix/) | Präfix für den Index des Arbeitsblatts. |
| [GetSplitPartPrefix](./getsplitpartprefix/) | Präfix für den Index des geteilten Teils. |
| [SetSplitPartPrefix](./setsplitpartprefix/) | Präfix für den Index des geteilten Teils. |
| [GetSheetIndexOffset](./getsheetindexoffset/) | Versatz des Blattindexes zwischen dem im Dateipfad verwendeten Wert und seinem tatsächlichen Wert (SplitPartInfo.SheetIndex). |
| [SetSheetIndexOffset](./setsheetindexoffset/) | Versatz des Blattindexes zwischen dem im Dateipfad verwendeten Wert und seinem tatsächlichen Wert (SplitPartInfo.SheetIndex). |
| [GetSplitPartIndexOffset](./getsplitpartindexoffset/) | Versatz des Indexes des geteilten Teils zwischen dem im Dateipfad verwendeten Wert und seinem tatsächlichen Wert (SplitPartInfo.PartIndex). |
| [SetSplitPartIndexOffset](./setsplitpartindexoffset/) | Versatz des Indexes des geteilten Teils zwischen dem im Dateipfad verwendeten Wert und seinem tatsächlichen Wert (SplitPartInfo.PartIndex). |
| [GetBuildPathWithSheetAlways](./getbuildpathwithsheetalways/) | Ob der Blattindex oder -name immer zum Dateipfad hinzugefügt wird. Standardwert ist false, das heißt, wenn nur ein Blatt vorhanden ist, werden der Blattindex (oder -name) und das entsprechende Präfix nicht zum Dateipfad hinzugefügt. |
| [SetBuildPathWithSheetAlways](./setbuildpathwithsheetalways/) | Ob der Blattindex oder -name immer zum Dateipfad hinzugefügt wird. Standardwert ist false, das heißt, wenn nur ein Blatt vorhanden ist, werden der Blattindex (oder -name) und das entsprechende Präfix nicht zum Dateipfad hinzugefügt. |
| [GetBuildPathWithSplitPartAlways](./getbuildpathwithsplitpartalways/) | Ob der Index des geteilten Teils immer zum Dateipfad hinzugefügt wird. Standardwert ist false, das heißt, wenn nur ein geteiltes Teil vorhanden ist, werden der Index des geteilten Teils und das entsprechende Präfix nicht zum Dateipfad hinzugefügt. |
| [SetBuildPathWithSplitPartAlways](./setbuildpathwithsplitpartalways/) | Ob der Index des geteilten Teils immer zum Dateipfad hinzugefügt wird. Standardwert ist false, das heißt, wenn nur ein geteiltes Teil vorhanden ist, werden der Index des geteilten Teils und das entsprechende Präfix nicht zum Dateipfad hinzugefügt. |
| [GetSaveOptionsTemplate](./getsaveoptionstemplate/) | Die Vorlage zum Erstellen einer Instanz von Speicheroptionen in GetSaveOptions(SplitPartInfo). |
| [SetSaveOptionsTemplate](./setsaveoptionstemplate/) | Die Vorlage zum Erstellen einer Instanz von Speicheroptionen in GetSaveOptions(SplitPartInfo). |
| [GetSaveOptions](./getsaveoptions/) | Ruft die Speicheroptionen ab, aus denen die Ausgabeeinstellungen für das aktuell geteilte Teil erhalten werden. |
| [Finish](./finish/) | Gibt Ressourcen nach der Verarbeitung des aktuell geteilten Teils frei. |
