---
title: "Klasse GridJsLogger"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridJs.GridJsLogger‑Klasse. Bietet ein leichtgewichtiges Protokollierungssystem für den GridJs‑Server. Unterstützt Konsolen‑ und Dateiausgabe mit konfigurierbaren Protokollstufen. Standardstufe ist Keine. Im DEBUG‑Build ist die Standardstufe Debug, die alle Meldungen ausgibt. Unterstützt das Rollen von Protokolldateien nach Tag/Woche/Monat."
type: docs
url: /de/net/aspose.cells.gridjs/gridjslogger/
---
## GridJsLogger class

Stellt ein leichtgewichtiges Protokollierungssystem für den GridJs‑Server bereit. Unterstützt Konsolen‑ und Dateiausgabe mit konfigurierbaren Protokollstufen. Standardstufe ist Keine. Im DEBUG‑Build ist die Standardstufe Debug (gibt alle Meldungen aus). Unterstützt das Rollen von Protokolldateien nach Tag/Woche/Monat.

```csharp
public static class GridJsLogger
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| static [EnableConsoleOutput](../../aspose.cells.gridjs/gridjslogger/enableconsoleoutput/) { get; set; } | Liest oder setzt, ob Lognachrichten in die Konsole ausgegeben werden sollen. Standard ist false. |
| static [EnableFileOutput](../../aspose.cells.gridjs/gridjslogger/enablefileoutput/) { get; set; } | Liest oder setzt, ob Lognachrichten in eine Datei geschrieben werden sollen. Standard ist false. [`SetLogFile`](./setlogfile/) oder [`SetLogDirectory`](./setlogdirectory/) muss vor dem Aktivieren aufgerufen werden. |
| static [Level](../../aspose.cells.gridjs/gridjslogger/level/) { get; set; } | Liest oder setzt das minimale Protokolllevel. Nachrichten unter diesem Level werden ignoriert. Standard ist None. |
| static [LogFilePath](../../aspose.cells.gridjs/gridjslogger/logfilepath/) { get; } | Liest den aktuellen Pfad der Logdatei oder null, wenn nicht gesetzt. |
| static [MaxFileSize](../../aspose.cells.gridjs/gridjslogger/maxfilesize/) { get; set; } | Liest oder setzt die maximale Größe (in Bytes) einer einzelnen Logdatei vor dem Rollen. Nur wirksam, wenn Rollen aktiviert ist. 0 bedeutet keine Größenbeschränkung. Standard ist 0. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| static [CloseLogFile](../../aspose.cells.gridjs/gridjslogger/closelogfile/)() | Schließt den Logdateischreiber und deaktiviert die Dateiausgabe. |
| static [Debug](../../aspose.cells.gridjs/gridjslogger/debug/)(string) | Protokolliert eine Debug‑Nachricht. |
| static [Error](../../aspose.cells.gridjs/gridjslogger/error/)(string) | Protokolliert eine Fehlermeldung. |
| static [Info](../../aspose.cells.gridjs/gridjslogger/info/)(string) | Protokolliert eine Informationsnachricht. |
| static [Log](../../aspose.cells.gridjs/gridjslogger/log/)(GridJsLogLevel, string) | Protokolliert eine Nachricht auf dem angegebenen Level. |
| static [SetLogDirectory](../../aspose.cells.gridjs/gridjslogger/setlogdirectory/#setlogdirectory)(string) | Setzt das Log‑Verzeichnis mit täglicher Rollstrategie und aktiviert die Dateiausgabe. Logdateien werden benannt als: gridjs_{period}.log |
| static [SetLogDirectory](../../aspose.cells.gridjs/gridjslogger/setlogdirectory/#setlogdirectory_1)(string, GridJsLogRolling) | Setzt das Log‑Verzeichnis mit Rollstrategie und aktiviert die Dateiausgabe. Logdateien werden benannt als: gridjs_{period}.log |
| static [SetLogDirectory](../../aspose.cells.gridjs/gridjslogger/setlogdirectory/#setlogdirectory_2)(string, GridJsLogRolling, string) | Setzt das Log‑Verzeichnis mit Rollstrategie und aktiviert die Dateiausgabe. Logdateien werden benannt als: {prefix}_{period}.log Beispiele: gridjs_2026-07-27.log (täglich), gridjs_2026-W30.log (wöchentlich), gridjs_2026-07.log (monatlich) |
| static [SetLogFile](../../aspose.cells.gridjs/gridjslogger/setlogfile/#setlogfile)(string) | Setzt den Pfad der Logdatei und aktiviert die Dateiausgabe (Einzeldateimodus, kein Rollen). Hängt an die bestehende Datei an. |
| static [SetLogFile](../../aspose.cells.gridjs/gridjslogger/setlogfile/#setlogfile_1)(string, bool) | Setzt den Pfad der Logdatei und aktiviert die Dateiausgabe (Einzeldateimodus, kein Rollen). |
| static [Warn](../../aspose.cells.gridjs/gridjslogger/warn/)(string) | Protokolliert eine Warnmeldung. |

### Siehe auch

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


