---
title: "AccessCacheOptions Enum"
linktitle: "AccessCacheOptions"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "AccessCacheOptions enum. Incapsula l'oggetto che rappresenta accesscacheoptions in Go."
type: docs
weight: 200
url: /it/go-cpp/accesscacheoptions/
---

## AccessCacheOptions Enum

Opzioni di caching per l'accesso ai dati. Più opzioni possono essere combinate usando l'operatore "|".

```go

type AccessCacheOptions int32


```

## Campi

| Campo | Descrizione |
| --- | --- |
| [None](./none/) | Nessuna cache per alcun accesso ai dati. |
| [All](./all/) | Applica tutte le ottimizzazioni possibili per tutti i tipi di accesso ai dati nella cartella di lavoro. Tutte le impostazioni e i dati non devono essere modificati durante l'accesso ottimizzato. |
| [PositionAndSize](./positionandsize/) | Applica l'ottimizzazione possibile per ottenere la posizione e le dimensioni dell'oggetto (ad esempio Shape). Le impostazioni dell'altezza delle righe e della larghezza delle colonne non devono essere modificate durante l'accesso ottimizzato. |
| [CellsData](./cellsdata/) | Applica l'ottimizzazione possibile per ottenere i valori delle celle. I dati delle celle (dati e impostazioni di Cell, Row) non devono essere modificati durante l'accesso ottimizzato, né devono essere creati nuovi oggetti Cell/Row (ad esempio tramite <see cref="Cells.this[int, int]"/>). |
| [CellDisplay](./celldisplay/) | Applica l'ottimizzazione possibile per ottenere i risultati relativi alla visualizzazione delle celle (<see cref="Cell.DisplayStringValue"/>, <see cref="Cell.GetStyle()"/>, <see cref="Cell.GetDisplayStyle()"/>, ecc.). I dati delle celle e gli oggetti relativi allo stile (stili di Cell/Row/Column, larghezza della colonna, ecc.) non devono essere modificati durante l'accesso ottimizzato. |
| [GetFormula](./getformula/) | Applica l'ottimizzazione possibile per ottenere le formule. Tutti i dati e le impostazioni che possono influenzare l'espressione della formula (nome del Worksheet, testo del Name, colonna della tabella, ecc.) non devono essere modificati durante l'accesso ottimizzato. |
| [SetFormula](./setformula/) | Applica l'ottimizzazione possibile per impostare le formule. Tutti i dati e le impostazioni che possono influenzare l'espressione della formula (nome del Worksheet, testo del Name, colonna della tabella, ecc.) non devono essere modificati durante l'accesso ottimizzato. |
| [CalculateFormula](./calculateformula/) | Applica l'ottimizzazione possibile per calcolare le formule. I dati delle celle non devono essere modificati durante l'accesso ottimizzato, né devono essere creati nuovi oggetti (Cell, Row, ecc.) (ad esempio tramite <see cref="Cells.this[int, int]"/>). |
| [ConditionalFormatting](./conditionalformatting/) | Applica l'ottimizzazione possibile per ottenere il risultato della formattazione condizionale. Tutti i dati e le impostazioni che possono influenzare il risultato delle formattazioni condizionali (impostazioni delle formattazioni condizionali, valori delle celle dipendenti, ecc.) non devono essere modificati durante l'accesso ottimizzato. |
| [Validation](./validation/) | Applica l'ottimizzazione possibile per ottenere il risultato della convalida. Tutti i dati e le impostazioni che possono influenzare il risultato della convalida (impostazioni della convalida, valori delle celle dipendenti, ecc.) non devono essere modificati durante l'accesso ottimizzato. |
