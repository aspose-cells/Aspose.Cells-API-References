---
title: Class GridJsLogger
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.GridJs.GridJsLogger class. Provides a lightweight logging system for GridJs server. Supports console and file output with configurable log levels. Default level is None. In DEBUG build the default level is Debug outputs all messages. Supports log file rolling by day/week/month
type: docs
url: /net/aspose.cells.gridjs/gridjslogger/
---
## GridJsLogger class

Provides a lightweight logging system for GridJs server. Supports console and file output with configurable log levels. Default level is None. In DEBUG build, the default level is Debug (outputs all messages). Supports log file rolling by day/week/month.

```csharp
public static class GridJsLogger
```

## Properties

| Name | Description |
| --- | --- |
| static [EnableConsoleOutput](../../aspose.cells.gridjs/gridjslogger/enableconsoleoutput/) { get; set; } | Gets or sets whether to output log messages to the console. Default is false. |
| static [EnableFileOutput](../../aspose.cells.gridjs/gridjslogger/enablefileoutput/) { get; set; } | Gets or sets whether to output log messages to a file. Default is false. Must call [`SetLogFile`](./setlogfile/) or [`SetLogDirectory`](./setlogdirectory/) before enabling. |
| static [Level](../../aspose.cells.gridjs/gridjslogger/level/) { get; set; } | Gets or sets the minimum log level. Messages below this level will be ignored. Default is None. |
| static [LogFilePath](../../aspose.cells.gridjs/gridjslogger/logfilepath/) { get; } | Gets the current log file path, or null if not set. |
| static [MaxFileSize](../../aspose.cells.gridjs/gridjslogger/maxfilesize/) { get; set; } | Gets or sets the maximum size (in bytes) for a single log file before rolling. Only effective when rolling is enabled. 0 means no size limit. Default is 0. |

## Methods

| Name | Description |
| --- | --- |
| static [CloseLogFile](../../aspose.cells.gridjs/gridjslogger/closelogfile/)() | Closes the log file writer and disables file output. |
| static [Debug](../../aspose.cells.gridjs/gridjslogger/debug/)(string) | Logs a debug level message. |
| static [Error](../../aspose.cells.gridjs/gridjslogger/error/)(string) | Logs an error level message. |
| static [Info](../../aspose.cells.gridjs/gridjslogger/info/)(string) | Logs an info level message. |
| static [Log](../../aspose.cells.gridjs/gridjslogger/log/)(GridJsLogLevel, string) | Logs a message at the specified level. |
| static [SetLogDirectory](../../aspose.cells.gridjs/gridjslogger/setlogdirectory/#setlogdirectory)(string) | Sets the log directory with daily rolling file strategy and enables file output. Log files will be named as: gridjs_{period}.log |
| static [SetLogDirectory](../../aspose.cells.gridjs/gridjslogger/setlogdirectory/#setlogdirectory_1)(string, GridJsLogRolling) | Sets the log directory with rolling file strategy and enables file output. Log files will be named as: gridjs_{period}.log |
| static [SetLogDirectory](../../aspose.cells.gridjs/gridjslogger/setlogdirectory/#setlogdirectory_2)(string, GridJsLogRolling, string) | Sets the log directory with rolling file strategy and enables file output. Log files will be named as: {prefix}_{period}.log Examples: gridjs_2026-07-27.log (Daily), gridjs_2026-W30.log (Weekly), gridjs_2026-07.log (Monthly) |
| static [SetLogFile](../../aspose.cells.gridjs/gridjslogger/setlogfile/#setlogfile)(string) | Sets the log file path and enables file output (single file mode, no rolling). Appends to existing file. |
| static [SetLogFile](../../aspose.cells.gridjs/gridjslogger/setlogfile/#setlogfile_1)(string, bool) | Sets the log file path and enables file output (single file mode, no rolling). |
| static [Warn](../../aspose.cells.gridjs/gridjslogger/warn/)(string) | Logs a warning level message. |

### See Also

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


