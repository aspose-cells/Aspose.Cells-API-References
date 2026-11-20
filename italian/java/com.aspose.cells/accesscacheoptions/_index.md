---
title: "AccessCacheOptions"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Opzioni di caching per l'accesso ai dati."
type: docs
url: /it/java/com.aspose.cells/accesscacheoptions/
---

**Inheritance:**
java.lang.Object
```
public final class AccessCacheOptions
```

Opzioni di caching per l'accesso ai dati. Più opzioni possono essere combinate usando l'operatore "\|".

**Remarks**

Per alcune funzionalità, l'accesso a grandi dataset richiede molte operazioni ripetute e complesse, come ricerca, calcolo, ecc., e tali operazioni richiedono molto tempo aggiuntivo. Nelle situazioni comuni, tutti i dati dipendenti rimangono invariati durante l'accesso, quindi è possibile creare e utilizzare alcune cache per migliorare le prestazioni di accesso. A questo scopo, forniamo questa API affinché l'utente possa specificare quale tipo di accesso ai dati debba essere ottimizzato mediante un possibile meccanismo di caching.

Si prega di notare che, per opzioni diverse, potrebbe essere necessario che diversi dataset siano "sola lettura". Inoltre, le prestazioni dell'accesso ai dati dipendono da molti fattori; l'uso del meccanismo di caching non garantisce un miglioramento delle prestazioni. In alcune situazioni, ad esempio quando il dataset da accedere è piccolo, l'utilizzo della cache può richiedere ancora più tempo, poiché il caching stesso necessita di tempo aggiuntivo.
## Campi

| Campo | Descrizione |
| --- | --- |
| [ALL](#ALL) | Applica tutte le ottimizzazioni possibili per tutti i tipi di accesso ai dati nella cartella di lavoro. |
| [CALCULATE_FORMULA](#CALCULATE-FORMULA) | Applica l'ottimizzazione possibile per il calcolo delle formule. |
| [CELLS_DATA](#CELLS-DATA) | Applica l'ottimizzazione possibile per l'ottenimento dei valori delle celle. |
| [CELL_DISPLAY](#CELL-DISPLAY) | Applica l'ottimizzazione possibile per l'ottenimento dei risultati relativi alla visualizzazione delle celle([Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--), [Cell.getStyle()](../../com.aspose.cells/cell\#getStyle--), [Cell.getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--), ecc.). |
| [CONDITIONAL_FORMATTING](#CONDITIONAL-FORMATTING) | Applica l'ottimizzazione possibile per l'ottenimento del risultato di formattazione delle formattazioni condizionali. |
| [GET_FORMULA](#GET-FORMULA) | Applica l'ottimizzazione possibile per l'ottenimento delle formule. |
| [NONE](#NONE) | Nessuna cache per alcun accesso ai dati. |
| [POSITION_AND_SIZE](#POSITION-AND-SIZE) | Applica l'ottimizzazione possibile per l'ottenimento della posizione e delle dimensioni dell'oggetto (ad esempio Shape). |
| [SET_FORMULA](#SET-FORMULA) | Applica l'ottimizzazione possibile per l'impostazione delle formule. |
| [VALIDATION](#VALIDATION) | Applica l'ottimizzazione possibile per l'ottenimento del risultato di convalida. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ALL {#ALL}
```
public static final int ALL
```


Applica tutte le ottimizzazioni possibili per tutti i tipi di accesso ai dati nella cartella di lavoro. Tutte le impostazioni e i dati non devono essere modificati durante l'accesso ottimizzato.

### CALCULATE_FORMULA {#CALCULATE-FORMULA}
```
public static final int CALCULATE_FORMULA
```


Applica l'ottimizzazione possibile per il calcolo delle formule. I dati delle celle non devono essere modificati durante l'accesso ottimizzato, né devono essere creati nuovi oggetti (Cell, Row, ecc.) (ad esempio tramite [Cells.get(int,int)](../../com.aspose.cells/cells\#get-int-int-)).

### CELLS_DATA {#CELLS-DATA}
```
public static final int CELLS_DATA
```


Applica l'ottimizzazione possibile per l'ottenimento dei valori delle celle. I dati delle celle (dati e impostazioni di Cell, Row) non devono essere modificati durante l'accesso ottimizzato, né devono essere creati nuovi oggetti Cell/Row (ad esempio tramite [Cells.get(int,int)](../../com.aspose.cells/cells\#get-int-int-)).

### CELL_DISPLAY {#CELL-DISPLAY}
```
public static final int CELL_DISPLAY
```


Applica l'ottimizzazione possibile per l'ottenimento dei risultati relativi alla visualizzazione delle celle([Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--), [Cell.getStyle()](../../com.aspose.cells/cell\#getStyle--), [Cell.getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--), ecc.). I dati delle celle e gli oggetti relativi allo stile (stili di Cell/Row/Column, larghezza della colonna, ecc.) non devono essere modificati durante l'accesso ottimizzato.

### CONDITIONAL_FORMATTING {#CONDITIONAL-FORMATTING}
```
public static final int CONDITIONAL_FORMATTING
```


Applica l'ottimizzazione possibile per ottenere il risultato della formattazione condizionale. Tutti i dati e le impostazioni che possono influenzare il risultato delle formattazioni condizionali (impostazioni delle formattazioni condizionali, valori delle celle dipendenti, ecc.) non devono essere modificati durante l'accesso ottimizzato.

### GET_FORMULA {#GET-FORMULA}
```
public static final int GET_FORMULA
```


Applica l'ottimizzazione possibile per ottenere le formule. Tutti i dati e le impostazioni che possono influenzare l'espressione della formula (nome del foglio di lavoro, testo del nome, colonna della tabella, ecc.) non devono essere modificati durante l'accesso ottimizzato.

### NONE {#NONE}
```
public static final int NONE
```


Nessuna cache per alcun accesso ai dati.

### POSITION_AND_SIZE {#POSITION-AND-SIZE}
```
public static final int POSITION_AND_SIZE
```


Applica l'ottimizzazione possibile per ottenere la posizione e le dimensioni dell'oggetto (ad esempio Shape). Le impostazioni dell'altezza delle righe e della larghezza delle colonne non devono essere modificate durante l'accesso ottimizzato.

### SET_FORMULA {#SET-FORMULA}
```
public static final int SET_FORMULA
```


Applica l'ottimizzazione possibile per impostare le formule. Tutti i dati e le impostazioni che possono influenzare l'espressione della formula (nome del foglio di lavoro, testo del nome, colonna della tabella, ecc.) non devono essere modificati durante l'accesso ottimizzato.

### VALIDATION {#VALIDATION}
```
public static final int VALIDATION
```


Applica l'ottimizzazione possibile per ottenere il risultato della convalida. Tutti i dati e le impostazioni che possono influenzare il risultato della convalida (impostazioni della convalida, valori delle celle dipendenti, ecc.) non devono essere modificati durante l'accesso ottimizzato.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

