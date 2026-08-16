---
title: GridJsLogger.SetLogDirectory
second_title: Aspose.Cells for .NET API Reference
description: GridJsLogger method. Sets the log directory with daily rolling file strategy and enables file output. Log files will be named as gridjs_period.log
type: docs
url: /net/aspose.cells.gridjs/gridjslogger/setlogdirectory/
---
## SetLogDirectory(string) {#setlogdirectory}

Sets the log directory with daily rolling file strategy and enables file output. Log files will be named as: gridjs_{period}.log

```csharp
public static void SetLogDirectory(string directory)
```

| Parameter | Type | Description |
| --- | --- | --- |
| directory | String | The directory to store log files. |

### See Also

* class [GridJsLogger](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)

---

## SetLogDirectory(string, GridJsLogRolling) {#setlogdirectory_1}

Sets the log directory with rolling file strategy and enables file output. Log files will be named as: gridjs_{period}.log

```csharp
public static void SetLogDirectory(string directory, GridJsLogRolling rolling)
```

| Parameter | Type | Description |
| --- | --- | --- |
| directory | String | The directory to store log files. |
| rolling | GridJsLogRolling | The rolling strategy (Daily/Weekly/Monthly). |

### See Also

* enum [GridJsLogRolling](../../gridjslogrolling/)
* class [GridJsLogger](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)

---

## SetLogDirectory(string, GridJsLogRolling, string) {#setlogdirectory_2}

Sets the log directory with rolling file strategy and enables file output. Log files will be named as: {prefix}_{period}.log Examples: gridjs_2026-07-27.log (Daily), gridjs_2026-W30.log (Weekly), gridjs_2026-07.log (Monthly)

```csharp
public static void SetLogDirectory(string directory, GridJsLogRolling rolling, string filePrefix)
```

| Parameter | Type | Description |
| --- | --- | --- |
| directory | String | The directory to store log files. |
| rolling | GridJsLogRolling | The rolling strategy (Daily/Weekly/Monthly). |
| filePrefix | String | The file name prefix. |

### See Also

* enum [GridJsLogRolling](../../gridjslogrolling/)
* class [GridJsLogger](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


