---
title: "类 GridJsLogger"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.GridJs.GridJsLogger 类。为 GridJs 服务器提供轻量级日志系统。支持带可配置日志级别的控制台和文件输出。默认级别为 None。调试构建中，默认级别为 Debug，输出所有消息。支持按天/周/月滚动日志文件。"
type: docs
url: /zh/net/aspose.cells.gridjs/gridjslogger/
---
## GridJsLogger class

为 GridJs 服务器提供轻量级日志系统。支持带可配置日志级别的控制台和文件输出。默认级别为 None。调试构建中，默认级别为 Debug（输出所有消息）。支持按天/周/月滚动日志文件。

```csharp
public static class GridJsLogger
```

## 属性

| 名称 | 描述 |
| --- | --- |
| static [EnableConsoleOutput](../../aspose.cells.gridjs/gridjslogger/enableconsoleoutput/) { get; set; } | 获取或设置是否将日志消息输出到控制台。默认值为 false。 |
| static [EnableFileOutput](../../aspose.cells.gridjs/gridjslogger/enablefileoutput/) { get; set; } | 获取或设置是否将日志消息输出到文件。默认值为 false。启用前必须调用 [`SetLogFile`](./setlogfile/) 或 [`SetLogDirectory`](./setlogdirectory/)。 |
| static [Level](../../aspose.cells.gridjs/gridjslogger/level/) { get; set; } | 获取或设置最小日志级别。低于此级别的消息将被忽略。默认值为 None。 |
| static [LogFilePath](../../aspose.cells.gridjs/gridjslogger/logfilepath/) { get; } | 获取当前日志文件路径，如果未设置则为 null。 |
| static [MaxFileSize](../../aspose.cells.gridjs/gridjslogger/maxfilesize/) { get; set; } | 获取或设置单个日志文件在滚动前的最大大小（字节）。仅在启用滚动时生效。0 表示无限制。默认值为 0。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| static [CloseLogFile](../../aspose.cells.gridjs/gridjslogger/closelogfile/)() | 关闭日志文件写入器并禁用文件输出。 |
| static [Debug](../../aspose.cells.gridjs/gridjslogger/debug/)(string) | 记录调试级别的消息。 |
| static [Error](../../aspose.cells.gridjs/gridjslogger/error/)(string) | 记录错误级别的消息。 |
| static [Info](../../aspose.cells.gridjs/gridjslogger/info/)(string) | 记录信息级别的消息。 |
| static [Log](../../aspose.cells.gridjs/gridjslogger/log/)(GridJsLogLevel, string) | 在指定级别记录一条消息。 |
| static [SetLogDirectory](../../aspose.cells.gridjs/gridjslogger/setlogdirectory/#setlogdirectory)(string) | 设置日志目录，使用每日滚动文件策略并启用文件输出。日志文件将命名为：gridjs_{period}.log |
| static [SetLogDirectory](../../aspose.cells.gridjs/gridjslogger/setlogdirectory/#setlogdirectory_1)(string, GridJsLogRolling) | 设置日志目录，使用滚动文件策略并启用文件输出。日志文件将命名为：gridjs_{period}.log |
| static [SetLogDirectory](../../aspose.cells.gridjs/gridjslogger/setlogdirectory/#setlogdirectory_2)(string, GridJsLogRolling, string) | 设置日志目录，使用滚动文件策略并启用文件输出。日志文件将命名为：{prefix}_{period}.log 示例：gridjs_2026-07-27.log（每日），gridjs_2026-W30.log（每周），gridjs_2026-07.log（每月） |
| static [SetLogFile](../../aspose.cells.gridjs/gridjslogger/setlogfile/#setlogfile)(string) | 设置日志文件路径并启用文件输出（单文件模式，无滚动）。追加到已有文件。 |
| static [SetLogFile](../../aspose.cells.gridjs/gridjslogger/setlogfile/#setlogfile_1)(string, bool) | 设置日志文件路径并启用文件输出（单文件模式，无滚动）。 |
| static [Warn](../../aspose.cells.gridjs/gridjslogger/warn/)(string) | 记录一条警告级别的消息。 |

### 另请参见

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


