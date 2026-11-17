---
title: "Classe CellsHelper"
linktitle: "CellsHelper"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe CellsHelper. Incapsula l'oggetto che rappresenta cellshelper in Go."
type: docs
weight: 200
url: /it/go-cpp/cellshelper/
---

## CellsHelper class

Fornisce funzioni di supporto.

```go

type CellsHelper struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [CellsHelper_GetSignificantDigitsType](./cellshelper_getsignificantdigitstype/) | Ottiene e imposta il tipo predefinito di cifre significative per l'emissione di valori numerici. Il valore predefinito è SignificantDigitsType.G17. |
| [CellsHelper_SetSignificantDigitsType](./cellshelper_setsignificantdigitstype/) | Ottiene e imposta il tipo predefinito di cifre significative per l'emissione di valori numerici. Il valore predefinito è SignificantDigitsType.G17. |
| [CellsHelper_GetDPI](./cellshelper_getdpi/) | Ottiene il DPI della macchina. |
| [CellsHelper_SetDPI](./cellshelper_setdpi/) | Ottiene il DPI della macchina. |
| [CellsHelper_GetTextWidth](./cellshelper_gettextwidth/) | Ottieni la larghezza del testo in unità di punti. |
| [CellsHelper_GetVersion](./cellshelper_getversion/) | Ottieni la versione di rilascio. |
| [CellsHelper_CellNameToIndex](./cellshelper_cellnametoindex/) | Ottiene gli indici di riga e colonna della cella in base al suo nome. |
| [CellsHelper_CellIndexToName](./cellshelper_cellindextoname/) | Ottiene il nome della cella in base ai suoi indici di riga e colonna. |
| [CellsHelper_ColumnIndexToName](./cellshelper_columnindextoname/) | Ottiene il nome della colonna in base all'indice della colonna. |
| [CellsHelper_ColumnNameToIndex](./cellshelper_columnnametoindex/) | Ottiene l'indice della colonna in base al nome della colonna. |
| [CellsHelper_RowIndexToName](./cellshelper_rowindextoname/) | Ottiene il nome della riga in base all'indice della riga. |
| [CellsHelper_RowNameToIndex](./cellshelper_rownametoindex/) | Ottiene l'indice della riga in base al nome della riga. |
| [CellsHelper_GetDateTimeFromDouble](./cellshelper_getdatetimefromdouble/) | Converti il valore double nel valore data/ora. |
| [CellsHelper_GetDoubleFromDateTime](./cellshelper_getdoublefromdatetime/) | Converti la data/ora in valore double. |
| [CellsHelper_GetStartupPath](./cellshelper_getstartuppath/) | Ottiene o imposta il percorso di avvio, a cui si fa riferimento da alcune formule esterne. |
| [CellsHelper_SetStartupPath](./cellshelper_setstartuppath/) | Ottiene o imposta il percorso di avvio, a cui si fa riferimento da alcune formule esterne. |
| [CellsHelper_GetAltStartPath](./cellshelper_getaltstartpath/) | Ottiene o imposta il percorso di avvio alternativo, a cui si fa riferimento da alcune formule esterne. |
| [CellsHelper_SetAltStartPath](./cellshelper_setaltstartpath/) | Ottiene o imposta il percorso di avvio alternativo, a cui si fa riferimento da alcune formule esterne. |
| [CellsHelper_GetLibraryPath](./cellshelper_getlibrarypath/) | Ottiene o imposta il percorso della libreria, a cui si fa riferimento da alcune formule esterne. |
| [CellsHelper_SetLibraryPath](./cellshelper_setlibrarypath/) | Ottiene o imposta il percorso della libreria, a cui si fa riferimento da alcune formule esterne. |
| [CellsHelper_GetUsedColors](./cellshelper_getusedcolors/) | Ottiene tutti i colori utilizzati nella cartella di lavoro. |
| [CellsHelper_MergeFiles](./cellshelper_mergefiles/) | Unisce alcuni file xls di grandi dimensioni in un file xls. |
| [CellsHelper_GetCacheFolder](./cellshelper_getcachefolder/) | Ottiene la cartella per i file temporanei che possono essere usati come cache dei dati. |
| [CellsHelper_SetCacheFolder](./cellshelper_setcachefolder/) | Imposta la cartella per i file temporanei che possono essere usati come cache dei dati. |
| [CellsHelper_CreateSafeSheetName_String](./cellshelper_createsafesheetname_string/) | Verifica il nome del foglio fornito e crea uno valido quando necessario. Se il nome del foglio fornito rispetta le regole dei nomi dei fogli Excel, lo restituisce. Altrimenti la stringa verrà troncata se la lunghezza supera il limite e i caratteri non validi saranno sostituiti con ' ', quindi verrà restituito il valore della stringa ricostruita. |
| [CellsHelper_CreateSafeSheetName_String_Char](./cellshelper_createsafesheetname_string_char/) | Verifica il nome del foglio fornito e crea uno valido quando necessario. Se il nome del foglio fornito rispetta le regole dei nomi dei fogli Excel, lo restituisce. Altrimenti la stringa verrà troncata se la lunghezza supera il limite e i caratteri non validi saranno sostituiti con il carattere fornito, quindi verrà restituito il valore della stringa ricostruita. |
| [CellsHelper_NeedQuoteInFormula](./cellshelper_needquoteinformula/) | Indica se il nome del foglio deve essere racchiuso tra virgolette singole |
| [CellsHelper_IsCloudPlatform](./cellshelper_iscloudplatform/) | Imposta questa proprietà su True quando si esegue su una piattaforma cloud, come: Azure, AWSLambda, ecc, |
| [CellsHelper_SetIsCloudPlatform](./cellshelper_setiscloudplatform/) | Imposta questa proprietà su True quando si esegue su una piattaforma cloud, come: Azure, AWSLambda, ecc, |
