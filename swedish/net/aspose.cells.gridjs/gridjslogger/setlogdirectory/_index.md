---
title: "GridJsLogger.SetLogDirectory"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridJsLogger-metod. Anger loggmappen med daglig rullningsstrategi för filer och aktiverar filutmatning. Loggfilerna kommer att namnges som gridjs_period.log"
type: docs
url: /sv/net/aspose.cells.gridjs/gridjslogger/setlogdirectory/
---
## SetLogDirectory(string) {#setlogdirectory}

Anger loggmappen med daglig rullningsstrategi och aktiverar filutmatning. Loggfilerna kommer att namnges som: gridjs_{period}.log

```csharp
public static void SetLogDirectory(string directory)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| katalog | String | Katalogen för att lagra loggfiler. |

### Se även

* class [GridJsLogger](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)

---

## SetLogDirectory(string, GridJsLogRolling) {#setlogdirectory_1}

Anger loggmappen med rullningsstrategi och aktiverar filutmatning. Loggfilerna kommer att namnges som: gridjs_{period}.log

```csharp
public static void SetLogDirectory(string directory, GridJsLogRolling rolling)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| katalog | String | Katalogen för att lagra loggfiler. |
| rullning | GridJsLogRolling | Rullningsstrategin (Daglig/Veckovis/Månatlig). |

### Se även

* enum [GridJsLogRolling](../../gridjslogrolling/)
* class [GridJsLogger](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)

---

## SetLogDirectory(string, GridJsLogRolling, string) {#setlogdirectory_2}

Anger loggmappen med rullningsstrategi och aktiverar filutmatning. Loggfilerna kommer att namnges som: {prefix}_{period}.log Exempel: gridjs_2026-07-27.log (Daglig), gridjs_2026-W30.log (Veckovis), gridjs_2026-07.log (Månatlig)

```csharp
public static void SetLogDirectory(string directory, GridJsLogRolling rolling, string filePrefix)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| katalog | String | Katalogen för att lagra loggfiler. |
| rullning | GridJsLogRolling | Rullningsstrategin (Daglig/Veckovis/Månatlig). |
| filePrefix | String | Filnamnsprefixet. |

### Se även

* enum [GridJsLogRolling](../../gridjslogrolling/)
* class [GridJsLogger](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


