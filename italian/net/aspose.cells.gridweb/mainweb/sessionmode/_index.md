---
title: "MainWeb.SessionMode"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "MainWeb property. Ottiene o imposta la modalità di sessione della griglia"
type: docs
url: /it/net/aspose.cells.gridweb/mainweb/sessionmode/
---
## MainWeb.SessionMode property

Ottiene o imposta la modalità di sessione della griglia.

```csharp
public SessionMode SessionMode { get; set; }
```

### Osservazioni

Esistono 4 tipi di modalità di sessione: 1. Session(default): Utilizza la sessione di sistema per memorizzare i dati del foglio. In genere asp.net utilizza lo stato di sessione InProc. La griglia supporta anche lo stato di sessione \"StateServer\" fuori processo e lo stato di sessione SQLServer. 2. ViewState: Utilizza il viewstate della pagina per memorizzare i dati del foglio. 3. Custom: Utilizza gli eventi LoadCustomData e SheetDataUpdated per memorizzare/ripristinare i dati del foglio. 4. File: memorizza/ripristina i dati del foglio in SessionStorePath. questo è il modo consigliato e può mantenere il file sempre. Quando si utilizza SessionMode.ViewState, la griglia memorizzerà alcuni dati nel viewstate della pagina. Questo ridurrà l'utilizzo di memoria del server, ma la dimensione della pagina sarà maggiore e influenzerà le prestazioni complessive.

### Esempi

```csharp
[C#]
	GridWeb1.SessionMode = SessionMode.ViewState;
	
[Visual Basic]
	GridWeb1.SessionMode = SessionMode.ViewState
```

### Vedi anche

* enum [SessionMode](../../sessionmode/)
* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


