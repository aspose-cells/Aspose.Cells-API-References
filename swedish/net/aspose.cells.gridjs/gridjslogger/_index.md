---
title: "Klass GridJsLogger"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridJs.GridJsLogger-klass. Tillhandahåller ett lättviktigt loggningssystem för GridJs-servern. Stöder konsol- och filutmatning med konfigurerbara loggningsnivåer. Standardnivån är None. I DEBUG-byggnad är standardnivån Debug och skriver ut alla meddelanden. Stöder rullning av loggfil per dag/vecka/månad."
type: docs
url: /sv/net/aspose.cells.gridjs/gridjslogger/
---
## GridJsLogger class

Tillhandahåller ett lättviktigt loggningssystem för GridJs-servern. Stöder konsol- och filutmatning med konfigurerbara loggnivåer. Standardnivån är Ingen. I DEBUG-bygg är standardnivån Debug (utskriver alla meddelanden). Stöder loggfilrullning per dag/vecka/månad.

```csharp
public static class GridJsLogger
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| static [EnableConsoleOutput](../../aspose.cells.gridjs/gridjslogger/enableconsoleoutput/) { get; set; } | Hämtar eller ställer in om loggmeddelanden ska skrivas ut till konsolen. Standard är false. |
| static [EnableFileOutput](../../aspose.cells.gridjs/gridjslogger/enablefileoutput/) { get; set; } | Hämtar eller ställer in om loggmeddelanden ska skrivas ut till en fil. Standard är false. Du måste anropa [`SetLogFile`](./setlogfile/) eller [`SetLogDirectory`](./setlogdirectory/) innan du aktiverar. |
| static [Level](../../aspose.cells.gridjs/gridjslogger/level/) { get; set; } | Hämtar eller anger den minsta loggnivån. Meddelanden under denna nivå kommer att ignoreras. Standard är Ingen. |
| static [LogFilePath](../../aspose.cells.gridjs/gridjslogger/logfilepath/) { get; } | Hämtar den aktuella sökvägen till loggfilen, eller null om den inte är angiven. |
| static [MaxFileSize](../../aspose.cells.gridjs/gridjslogger/maxfilesize/) { get; set; } | Hämtar eller anger den maximala storleken (i byte) för en enskild loggfil innan den rullas. Gäller endast när rullning är aktiverad. 0 betyder ingen storleksgräns. Standard är 0. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| static [CloseLogFile](../../aspose.cells.gridjs/gridjslogger/closelogfile/)() | Stänger loggfilsskrivaren och inaktiverar filutmatning. |
| static [Debug](../../aspose.cells.gridjs/gridjslogger/debug/)(string) | Loggar ett meddelande på debug-nivå. |
| static [Error](../../aspose.cells.gridjs/gridjslogger/error/)(string) | Loggar ett meddelande på felnivå. |
| static [Info](../../aspose.cells.gridjs/gridjslogger/info/)(string) | Loggar ett meddelande på informationsnivå. |
| static [Log](../../aspose.cells.gridjs/gridjslogger/log/)(GridJsLogLevel, string) | Loggar ett meddelande på den angivna nivån. |
| static [SetLogDirectory](../../aspose.cells.gridjs/gridjslogger/setlogdirectory/#setlogdirectory)(string) | Anger loggmappen med daglig rullningsstrategi och aktiverar filutmatning. Loggfilerna kommer att namnges som: gridjs_{period}.log |
| static [SetLogDirectory](../../aspose.cells.gridjs/gridjslogger/setlogdirectory/#setlogdirectory_1)(string, GridJsLogRolling) | Anger loggmappen med rullningsstrategi och aktiverar filutmatning. Loggfilerna kommer att namnges som: gridjs_{period}.log |
| static [SetLogDirectory](../../aspose.cells.gridjs/gridjslogger/setlogdirectory/#setlogdirectory_2)(string, GridJsLogRolling, string) | Anger loggmappen med rullningsstrategi och aktiverar filutmatning. Loggfilerna kommer att namnges som: {prefix}_{period}.log Exempel: gridjs_2026-07-27.log (Daglig), gridjs_2026-W30.log (Veckovis), gridjs_2026-07.log (Månatlig) |
| static [SetLogFile](../../aspose.cells.gridjs/gridjslogger/setlogfile/#setlogfile)(string) | Anger sökvägen till loggfilen och aktiverar filutmatning (enkel fil-läge, ingen rullning). Lägger till i befintlig fil. |
| static [SetLogFile](../../aspose.cells.gridjs/gridjslogger/setlogfile/#setlogfile_1)(string, bool) | Anger sökvägen till loggfilen och aktiverar filutmatning (enkel fil-läge, ingen rullning). |
| static [Warn](../../aspose.cells.gridjs/gridjslogger/warn/)(string) | Loggar ett meddelande på varningsnivå. |

### Se även

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


