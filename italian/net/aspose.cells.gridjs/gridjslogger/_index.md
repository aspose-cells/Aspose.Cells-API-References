---
title: "Classe GridJsLogger"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.GridJs.GridJsLogger. Fornisce un sistema di registrazione leggero per il server GridJs. Supporta l'output su console e file con livelli di log configurabili. Il livello predefinito è None. Nella build DEBUG il livello predefinito è Debug e visualizza tutti i messaggi. Supporta il rollover dei file di log per giorno/settimana/mese."
type: docs
url: /it/net/aspose.cells.gridjs/gridjslogger/
---
## GridJsLogger class

Fornisce un sistema di logging leggero per il server GridJs. Supporta l'output su console e file con livelli di log configurabili. Il livello predefinito è None. In build DEBUG, il livello predefinito è Debug (genera tutti i messaggi). Supporta il rollover dei file di log per giorno/settimana/mese.

```csharp
public static class GridJsLogger
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| static [EnableConsoleOutput](../../aspose.cells.gridjs/gridjslogger/enableconsoleoutput/) { get; set; } | Ottiene o imposta se inviare i messaggi di log alla console. Il valore predefinito è false. |
| static [EnableFileOutput](../../aspose.cells.gridjs/gridjslogger/enablefileoutput/) { get; set; } | Ottiene o imposta se inviare i messaggi di log a un file. Il valore predefinito è false. È necessario chiamare [`SetLogFile`](./setlogfile/) o [`SetLogDirectory`](./setlogdirectory/) prima di abilitare. |
| static [Level](../../aspose.cells.gridjs/gridjslogger/level/) { get; set; } | Ottiene o imposta il livello minimo di log. I messaggi al di sotto di questo livello verranno ignorati. Il valore predefinito è None. |
| static [LogFilePath](../../aspose.cells.gridjs/gridjslogger/logfilepath/) { get; } | Ottiene il percorso corrente del file di log, o null se non impostato. |
| static [MaxFileSize](../../aspose.cells.gridjs/gridjslogger/maxfilesize/) { get; set; } | Ottiene o imposta la dimensione massima (in byte) per un singolo file di log prima del rollover. È efficace solo quando il rollover è abilitato. 0 significa nessun limite di dimensione. Il valore predefinito è 0. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [CloseLogFile](../../aspose.cells.gridjs/gridjslogger/closelogfile/)() | Chiude lo scrittore del file di log e disabilita l'output su file. |
| static [Debug](../../aspose.cells.gridjs/gridjslogger/debug/)(string) | Registra un messaggio a livello debug. |
| static [Error](../../aspose.cells.gridjs/gridjslogger/error/)(string) | Registra un messaggio a livello errore. |
| static [Info](../../aspose.cells.gridjs/gridjslogger/info/)(string) | Registra un messaggio a livello informazione. |
| static [Log](../../aspose.cells.gridjs/gridjslogger/log/)(GridJsLogLevel, string) | Registra un messaggio al livello specificato. |
| static [SetLogDirectory](../../aspose.cells.gridjs/gridjslogger/setlogdirectory/#setlogdirectory)(string) | Imposta la directory dei log con strategia di rollover giornaliero e abilita l'output su file. I file di log saranno nominati così: gridjs_{period}.log |
| static [SetLogDirectory](../../aspose.cells.gridjs/gridjslogger/setlogdirectory/#setlogdirectory_1)(string, GridJsLogRolling) | Imposta la directory dei log con strategia di rollover e abilita l'output su file. I file di log saranno nominati così: gridjs_{period}.log |
| static [SetLogDirectory](../../aspose.cells.gridjs/gridjslogger/setlogdirectory/#setlogdirectory_2)(string, GridJsLogRolling, string) | Imposta la directory dei log con strategia di rollover e abilita l'output su file. I file di log saranno nominati così: {prefix}_{period}.log Esempi: gridjs_2026-07-27.log (Giornaliero), gridjs_2026-W30.log (Settimanale), gridjs_2026-07.log (Mensile) |
| static [SetLogFile](../../aspose.cells.gridjs/gridjslogger/setlogfile/#setlogfile)(string) | Imposta il percorso del file di log e abilita l'output su file (modalità singolo file, senza rollover). Aggiunge al file esistente. |
| static [SetLogFile](../../aspose.cells.gridjs/gridjslogger/setlogfile/#setlogfile_1)(string, bool) | Imposta il percorso del file di log e abilita l'output su file (modalità singolo file, senza rollover). |
| static [Warn](../../aspose.cells.gridjs/gridjslogger/warn/)(string) | Registra un messaggio di livello di avviso. |

### Vedi anche

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


