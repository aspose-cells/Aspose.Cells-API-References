---
title: "GridJsLogger.SetLogDirectory"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "GridJsLogger 方法。设置使用每日滚动文件策略的日志目录并启用文件输出。日志文件将命名为 gridjs_period.log"
type: docs
url: /zh/net/aspose.cells.gridjs/gridjslogger/setlogdirectory/
---
## SetLogDirectory(string) {#setlogdirectory}

设置日志目录，使用每日滚动文件策略并启用文件输出。日志文件将命名为：gridjs_{period}.log

```csharp
public static void SetLogDirectory(string directory)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| directory | String | 用于存储日志文件的目录。 |

### 另请参见

* class [GridJsLogger](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)

---

## SetLogDirectory(string, GridJsLogRolling) {#setlogdirectory_1}

设置日志目录，使用滚动文件策略并启用文件输出。日志文件将命名为：gridjs_{period}.log

```csharp
public static void SetLogDirectory(string directory, GridJsLogRolling rolling)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| directory | String | 用于存储日志文件的目录。 |
| rolling | GridJsLogRolling | 滚动策略（每日/每周/每月）。 |

### 另请参见

* enum [GridJsLogRolling](../../gridjslogrolling/)
* class [GridJsLogger](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)

---

## SetLogDirectory(string, GridJsLogRolling, string) {#setlogdirectory_2}

设置日志目录，使用滚动文件策略并启用文件输出。日志文件将命名为：{prefix}_{period}.log 示例：gridjs_2026-07-27.log（每日），gridjs_2026-W30.log（每周），gridjs_2026-07.log（每月）

```csharp
public static void SetLogDirectory(string directory, GridJsLogRolling rolling, string filePrefix)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| directory | String | 用于存储日志文件的目录。 |
| rolling | GridJsLogRolling | 滚动策略（每日/每周/每月）。 |
| filePrefix | String | 文件名前缀。 |

### 另请参见

* enum [GridJsLogRolling](../../gridjslogrolling/)
* class [GridJsLogger](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


