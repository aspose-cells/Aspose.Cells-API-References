---
title: AccessCacheOptions enumerazione
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 1740
url: /it/python-net/aspose.cells/accesscacheoptions/
is_root: false
---
##  AccessCacheOptions enumerazione
Opzioni di cache per l'accesso ai dati. Combinabile con | operatore per più opzioni insieme.



Il tipo AccessCacheOptions espone i membri seguenti:

###  Campi
| Campo| Descrizione|
| :- | :- |
| NONE | Nessuna cache per qualsiasi accesso ai dati.|
| ALL | Applicare tutte le possibili ottimizzazioni per tutti i tipi di accesso ai dati nella cartella di lavoro.<br/> Tutte le impostazioni e i dati non devono essere modificati durante l'accesso ottimizzato.|
| POSITION_AND_SIZE | Applica la possibile ottimizzazione per ottenere la posizione e le dimensioni dell'oggetto (come Shape).<br/> Le impostazioni dell'altezza della riga e della larghezza della colonna non devono essere modificate durante l'accesso ottimizzato.|
| CELLS_DATA | Applica la possibile ottimizzazione per ottenere i valori delle celle.<br/>Cells data(dati e impostazioni di Cell, Riga) non devono essere modificati durante<br/>l'accesso ottimizzato, non devono essere creati nemmeno nuovi oggetti Cell/Row (come<br/> da [[indicizzatore]](/cells/python-net/aspose.cells/cells/__getitem__/)).|
| CELL_DISPLAY | Applica la possibile ottimizzazione per ottenere risultati relativi alla visualizzazione di<br/>celle ([Cell.display_string_value](/cells/it/python-net/aspose.cells/cell#display_string_value), [Cell.get_style()](/cells/it/python-net/aspose.cells/cell/get_style), [Cell.get_display_style()](/cells/it/python-net/aspose.cells/cell/get_display_style), ecc.).<br/>Cells dati e oggetti relativi allo stile (stili Cell/riga/colonna, larghezza colonna, ecc.) non devono essere modificati<br/>durante l'accesso ottimizzato.|
| GET_FORMULA | Applicare possibile ottimizzazione per ottenere formule.<br/>Tutti i dati e le impostazioni che possono influire sull'espressione della formula (nome del foglio di lavoro, testo del nome,<br/> colonna della tabella, ecc.) non devono essere modificati durante l'accesso ottimizzato.|
| SET_FORMULA | Applicare l'eventuale ottimizzazione per l'impostazione delle formule.<br/>Tutti i dati e le impostazioni che possono influire sull'espressione della formula (nome del foglio di lavoro, testo del nome,<br/> colonna della tabella, ecc.) non devono essere modificati durante l'accesso ottimizzato.|
| CALCULATE_FORMULA | Applicare possibili ottimizzazioni per il calcolo delle formule.<br/>Cells i dati non devono essere modificati durante l'accesso ottimizzato, nessun nuovo oggetto (Cell, riga, ecc.)<br/> dovrebbe essere creato (come da [[indexer]](/cells/python-net/aspose.cells/cells/__getitem__/)).|
| CONDITIONAL_FORMATTING | Applica la possibile ottimizzazione per ottenere il risultato della formattazione delle formattazioni condizionali.<br/>Tutti i dati e le impostazioni che possono influenzare il risultato delle formattazioni condizionali (impostazioni di<br/> formattazioni condizionali, valori delle celle dipendenti, ecc.) non devono essere modificati durante l'accesso ottimizzato.|
| VALIDATION | Applica la possibile ottimizzazione per ottenere il risultato della convalida.<br/>Tutti i dati e le impostazioni che possono influenzare il risultato della convalida (impostazioni della convalida,<br/> valori delle celle dipendenti, ecc.) non devono essere modificati durante l'accesso ottimizzato.|



###  Osservazioni

Per alcune funzionalità, l'accesso a set di dati di grandi dimensioni richiede molte operazioni ripetute e complicate
come la ricerca, il calcolo, ecc. e queste operazioni richiederanno molto tempo in più.
Per situazioni comuni, tutti i dati dipendenti rimangono invariati durante l'accesso, quindi è possibile creare e utilizzare alcune cache
migliorare le prestazioni di accesso.
A tale scopo, forniamo questo API in modo che l'utente possa specificare quale tipo di accesso ai dati necessita
essere ottimizzato da un possibile meccanismo di memorizzazione nella cache.


Si prega di notare che per diverse opzioni, potrebbe essere necessario che diversi set di dati siano "di sola lettura".
E le prestazioni di accesso ai dati dipendono da molti aspetti, l'uso del meccanismo di memorizzazione nella cache
non garantisce che le prestazioni saranno migliorate. Per alcune situazioni,
come il set di dati a cui accedere è piccolo, l'utilizzo della cache può causare ancora più tempo perché
anche la memorizzazione nella cache richiede un certo tempo extra.

###  Guarda anche
* modulo [aspose.cells](..)
