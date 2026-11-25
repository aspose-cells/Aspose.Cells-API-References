---
title: "GridJsLogger.SetLogDirectory"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "GridJsLogger metodo. Imposta la directory dei log con strategia di rotazione giornaliera dei file e abilita l'output su file. I file di log saranno nominati come gridjs_period.log"
type: docs
url: /it/net/aspose.cells.gridjs/gridjslogger/setlogdirectory/
---
## SetLogDirectory(string) {#setlogdirectory}

Imposta la directory dei log con strategia di rollover giornaliero e abilita l'output su file. I file di log saranno nominati così: gridjs_{period}.log

```csharp
public static void SetLogDirectory(string directory)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| directory | String | La directory in cui memorizzare i file di log. |

### Vedi anche

* class [GridJsLogger](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)

---

## SetLogDirectory(string, GridJsLogRolling) {#setlogdirectory_1}

Imposta la directory dei log con strategia di rollover e abilita l'output su file. I file di log saranno nominati così: gridjs_{period}.log

```csharp
public static void SetLogDirectory(string directory, GridJsLogRolling rolling)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| directory | String | La directory in cui memorizzare i file di log. |
| rotazione | GridJsLogRolling | La strategia di rotazione (Daily/Weekly/Monthly). |

### Vedi anche

* enum [GridJsLogRolling](../../gridjslogrolling/)
* class [GridJsLogger](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)

---

## SetLogDirectory(string, GridJsLogRolling, string) {#setlogdirectory_2}

Imposta la directory dei log con strategia di rollover e abilita l'output su file. I file di log saranno nominati così: {prefix}_{period}.log Esempi: gridjs_2026-07-27.log (Giornaliero), gridjs_2026-W30.log (Settimanale), gridjs_2026-07.log (Mensile)

```csharp
public static void SetLogDirectory(string directory, GridJsLogRolling rolling, string filePrefix)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| directory | String | La directory in cui memorizzare i file di log. |
| rotazione | GridJsLogRolling | La strategia di rotazione (Daily/Weekly/Monthly). |
| filePrefix | String | Il prefisso del nome file. |

### Vedi anche

* enum [GridJsLogRolling](../../gridjslogrolling/)
* class [GridJsLogger](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


