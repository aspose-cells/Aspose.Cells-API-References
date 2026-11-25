---
title: "Aspose.Cells.GridJs"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Il namespace Aspose.Cells.GridJs incapsula tutte le classi di GridJs fornendo API semplici per visualizzare o modificare i file di fogli di calcolo tramite operazioni JSON"
type: docs
url: /it/net/aspose.cells.gridjs/
---
Il namespace **Aspose.Cells.GridJs** incapsula tutte le classi di GridJs, fornendo API semplici per visualizzare o modificare file di fogli di calcolo tramite operazioni JSON.

## Classi

| Classe | Descrizione |
| --- | --- |
| [Config](./config/) | Rappresenta tutte le impostazioni statiche per GridJs |
| [DefaultGridJsJsonCache](./defaultgridjsjsoncache/) | Implementazione predefinita della cache JSON (L1 memoria + L2 disco) |
| [GridAbstractCalculationEngine](./gridabstractcalculationengine/) | Rappresenta il motore di calcolo personalizzato dell'utente per estendere il motore di calcolo predefinito di **Aspose.Cells**. |
| [GridCacheForStream](./gridcacheforstream/) | Questa classe contiene le operazioni di cache per GridJs. L'utente deve implementare la propria logica di business per l'archiviazione basandosi su di essa.. |
| [GridCalculationData](./gridcalculationdata/) | Rappresenta i dati richiesti durante il calcolo di una funzione, come il nome della funzione, i parametri, ...ecc. |
| [GridCellException](./gridcellexception/) | L'eccezione che viene lanciata quando si verifica un errore specificato da GridJs. |
| [GridInterruptMonitor](./gridinterruptmonitor/) | Rappresenta tutti gli operatori relativi all'interruzione del calcolo. |
| [GridJsControllerBase](./gridjscontrollerbase/) |  |
| [GridJsLogger](./gridjslogger/) | Fornisce un sistema di logging leggero per il server GridJs. Supporta l'output su console e file con livelli di log configurabili. Il livello predefinito è None. In build DEBUG, il livello predefinito è Debug (genera tutti i messaggi). Supporta il rollover dei file di log per giorno/settimana/mese. |
| [GridJsOptions](./gridjsoptions/) | Rappresenta tutte le opzioni di caricamento per GridJs |
| [GridJsPermissionException](./gridjspermissionexception/) | rappresenta un'eccezione di permesso nella modalità collaborativa. Disponibile solo nella versione Java al momento, sarà disponibile nelle versioni .net/python in futuro. |
| [GridJsService](./gridjsservice/) | Fornisce le API operative di base utilizzate nelle azioni del controller. |
| [GridJsWorkbook](./gridjsworkbook/) | Rappresenta la classe principale di ingresso per GridJs |
| [GridReferredArea](./gridreferredarea/) | Rappresenta un'area di riferimento della formula. |
| [GridUpdateMonitor](./gridupdatemonitor/) | Monitor per l'utente per tracciare le modifiche dell'operazione di aggiornamento. |
| [GridWorkbookSettings](./gridworkbooksettings/) | Rappresenta le impostazioni della cartella di lavoro. |
| [JsonCacheOptions](./jsoncacheoptions/) | Opzioni di configurazione per la cache JSON in GridJs. Controlla il comportamento della cache sia in memoria (L1) che su disco (L2). |
| [OprMessageService](./oprmessageservice/) | Questa classe fornisce tutte le operazioni per la sincronizzazione dei messaggi in modalità collaborativa. |
## Interfacce

| Interfaccia | Descrizione |
| --- | --- |
| [CoWorkUserProvider](./coworkuserprovider/) | Rappresenta l'interfaccia del provider utente nella modalità collaborativa. Disponibile solo nella versione Java al momento, sarà disponibile nelle versioni .net/python in futuro. L'applicazione cliente può implementare questa interfaccia per fornire le informazioni sull'utente. |
| [IGridJsJsonCache](./igridjsjsoncache/) | Interfaccia della cache JSON - i clienti implementano strategie di archiviazione e invalidazione specifiche |
| [IGridJsService](./igridjsservice/) | Rappresenta l'interfaccia delle API operative di base utilizzate nelle azioni del controller. |
| [ITextTranslator](./itexttranslator/) | Rappresenta l'interfaccia per la traduzione |
## Enumerazione

| Enumerazione | Descrizione |
| --- | --- |
| [CoWorkOperationType](./coworkoperationtype/) | Rappresenta il tipo di operazione d'azione nella modalità collaborativa. Disponibile solo nella versione Java al momento, sarà disponibile nelle versioni .net/python in futuro. |
| [CoWorkUserPermission](./coworkuserpermission/) | rappresenta il permesso dell'utente nella modalità collaborativa. Disponibile solo nella versione Java al momento, sarà disponibile nelle versioni .net/python in futuro. |
| [GridExceptionType](./gridexceptiontype/) | Rappresenta il codice di eccezione personalizzato per GridJs. |
| [GridJsLogLevel](./gridjsloglevel/) | Specifica il livello di log per il logging di GridJs. |
| [GridJsLogRolling](./gridjslogrolling/) | Specifica la strategia di rollover del file di log. |
| [GridLoadFormat](./gridloadformat/) | Rappresenta il formato di caricamento del file. |


