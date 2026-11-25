---
title: "Enum AccessCacheOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.AccessCacheOptions enum. Opzioni di cache per l'accesso ai dati. Più opzioni possono essere combinate usando l'operatore "
type: docs
url: /it/net/aspose.cells/accesscacheoptions/
---
## AccessCacheOptions enumeration

Opzioni di caching per l'accesso ai dati. Più opzioni possono essere combinate usando l'operatore "&#x7C;".

```csharp
[Flags]
public enum AccessCacheOptions
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Nessuna cache per alcun accesso ai dati. |
| All | `FFFFFFFFFFFFFFFF` | Applica tutte le ottimizzazioni possibili per tutti i tipi di accesso ai dati nella cartella di lavoro. Tutte le impostazioni e i dati non devono essere modificati durante l'accesso ottimizzato. |
| PositionAndSize | `3` | Applica un'eventuale ottimizzazione per ottenere la posizione e le dimensioni dell'oggetto (ad esempio Shape). Le impostazioni dell'altezza della riga e della larghezza della colonna non devono essere modificate durante l'accesso ottimizzato. |
| CellsData | `9` | Applica un'eventuale ottimizzazione per ottenere i valori delle celle. I dati delle celle (dati e impostazioni di Cell, Row) non devono essere modificati durante l'accesso ottimizzato; non devono essere creati nuovi oggetti Cell/Row (ad esempio tramite [`Item`](../cells/item/)). |
| CellDisplay | `100086` | Applica un'eventuale ottimizzazione per ottenere i risultati relativi alla visualizzazione delle celle ([`DisplayStringValue`](../cell/displaystringvalue/), [`GetStyle`](../cell/getstyle/), [`GetDisplayStyle`](../cell/getdisplaystyle/), ecc.). I dati delle celle e gli oggetti relativi allo stile (stili di Cell/Row/Column, larghezza della colonna, ecc.) non devono essere modificati durante l'accesso ottimizzato. |
| GetFormula | `200000` | Applica un'eventuale ottimizzazione per ottenere le formule. Tutti i dati e le impostazioni che possono influenzare l'espressione della formula (nome del Worksheet, testo del Name, colonna della tabella, ecc.) non devono essere modificati durante l'accesso ottimizzato. |
| SetFormula | `400000` | Applica un'eventuale ottimizzazione per impostare le formule. Tutti i dati e le impostazioni che possono influenzare l'espressione della formula (nome del Worksheet, testo del Name, colonna della tabella, ecc.) non devono essere modificati durante l'accesso ottimizzato. |
| CalculateFormula | `800009` | Applica un'eventuale ottimizzazione per calcolare le formule. I dati delle celle non devono essere modificati durante l'accesso ottimizzato; non devono essere creati nuovi oggetti (Cell, Row, ecc.) (ad esempio tramite [`Item`](../cells/item/)). |
| ConditionalFormatting | `1000009` | Applica un'eventuale ottimizzazione per ottenere il risultato della formattazione condizionale. Tutti i dati e le impostazioni che possono influenzare il risultato della formattazione condizionale (impostazioni della formattazione condizionale, valori delle celle dipendenti, ecc.) non devono essere modificati durante l'accesso ottimizzato. |
| Validation | `2000009` | Applica un'eventuale ottimizzazione per ottenere il risultato della convalida. Tutti i dati e le impostazioni che possono influenzare il risultato della convalida (impostazioni della convalida, valori delle celle dipendenti, ecc.) non devono essere modificati durante l'accesso ottimizzato. |

### Osservazioni

Per alcune funzionalità, l'accesso a un grande set di dati richiede molte operazioni ripetute e complesse, come la ricerca, il calcolo, ecc., e tali operazioni richiedono molto tempo aggiuntivo. Nelle situazioni comuni, tutti i dati dipendenti rimangono invariati durante l'accesso, quindi è possibile creare e utilizzare alcune cache per migliorare le prestazioni dell'accesso. A tal fine, forniamo questa API affinché l'utente possa specificare quale tipo di accesso ai dati debba essere ottimizzato mediante un meccanismo di caching. Si noti che, per opzioni diverse, potrebbe essere necessario che diversi set di dati siano "read-only". Inoltre, le prestazioni dell'accesso ai dati dipendono da molti fattori; l'uso del meccanismo di caching non garantisce un miglioramento delle prestazioni. In alcune situazioni, ad esempio quando il set di dati da accedere è piccolo, l'uso della cache può richiedere più tempo, poiché il caching stesso richiede un certo tempo aggiuntivo.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AccessCacheOptionsDemo
    {
        public static void AccessCacheOptionsExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Avvia la cache di accesso con opzioni specifiche
            workbook.StartAccessCache(AccessCacheOptions.PositionAndSize | AccessCacheOptions.CellsData);

            // Esegui alcune operazioni che beneficiano del caching
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue(i + j);
                }
            }

            // Chiudi la cache di accesso
            workbook.CloseAccessCache(AccessCacheOptions.PositionAndSize | AccessCacheOptions.CellsData);

            // Salva la cartella di lavoro
            workbook.Save("AccessCacheOptionsExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


