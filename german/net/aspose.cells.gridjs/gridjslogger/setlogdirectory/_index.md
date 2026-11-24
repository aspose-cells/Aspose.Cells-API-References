---
title: "GridJsLogger.SetLogDirectory"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridJsLogger-Methode. Legt das Protokollverzeichnis mit täglicher rollierender Dateistrategie fest und aktiviert die Dateiausgabe. Protokolldateien werden als gridjs_period.log benannt."
type: docs
url: /de/net/aspose.cells.gridjs/gridjslogger/setlogdirectory/
---
## SetLogDirectory(string) {#setlogdirectory}

Setzt das Log‑Verzeichnis mit täglicher Rollstrategie und aktiviert die Dateiausgabe. Logdateien werden benannt als: gridjs_{period}.log

```csharp
public static void SetLogDirectory(string directory)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Verzeichnis | String | Das Verzeichnis, in dem Protokolldateien gespeichert werden. |

### Siehe auch

* class [GridJsLogger](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)

---

## SetLogDirectory(string, GridJsLogRolling) {#setlogdirectory_1}

Setzt das Log‑Verzeichnis mit Rollstrategie und aktiviert die Dateiausgabe. Logdateien werden benannt als: gridjs_{period}.log

```csharp
public static void SetLogDirectory(string directory, GridJsLogRolling rolling)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Verzeichnis | String | Das Verzeichnis, in dem Protokolldateien gespeichert werden. |
| rollierend | GridJsLogRolling | Die Rollierungsstrategie (Täglich/Wöchentlich/Monatlich). |

### Siehe auch

* enum [GridJsLogRolling](../../gridjslogrolling/)
* class [GridJsLogger](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)

---

## SetLogDirectory(string, GridJsLogRolling, string) {#setlogdirectory_2}

Setzt das Log‑Verzeichnis mit Rollstrategie und aktiviert die Dateiausgabe. Logdateien werden benannt als: {prefix}_{period}.log Beispiele: gridjs_2026-07-27.log (täglich), gridjs_2026-W30.log (wöchentlich), gridjs_2026-07.log (monatlich)

```csharp
public static void SetLogDirectory(string directory, GridJsLogRolling rolling, string filePrefix)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Verzeichnis | String | Das Verzeichnis, in dem Protokolldateien gespeichert werden. |
| rollierend | GridJsLogRolling | Die Rollierungsstrategie (Täglich/Wöchentlich/Monatlich). |
| DateiPräfix | String | Der Präfix des Dateinamens. |

### Siehe auch

* enum [GridJsLogRolling](../../gridjslogrolling/)
* class [GridJsLogger](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


