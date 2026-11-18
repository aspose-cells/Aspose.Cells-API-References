---
title: "PasteOptions-klass"
linktitle: "PasteOptions"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "PasteOptions-klass. Inkapslar objektet som representerar pasteoptions i Go."
type: docs
weight: 200
url: /sv/go-cpp/pasteoptions/
---

## PasteOptions class

Representerar alternativen för klistra in special.

```go

type PasteOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewPasteOptions](./newpasteoptions/) | Standardkonstruktor. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetPasteType](./getpastetype/) | Den speciella inklistringstypen. |
| [SetPasteType](./setpastetype/) | Den speciella inklistringstypen. |
| [GetShiftFormulasOfShapes](./getshiftformulasofshapes/) | Anger om formlerna för formerna ska förskjutas när områden kopieras. |
| [SetShiftFormulasOfShapes](./setshiftformulasofshapes/) | Anger om formlerna för formerna ska förskjutas när områden kopieras. |
| [GetSkipBlanks](./getskipblanks/) | Anger om tomma celler ska hoppas över. |
| [SetSkipBlanks](./setskipblanks/) | Anger om tomma celler ska hoppas över. |
| [GetKeepOldTables](./getkeepoldtables/) | Behåller tabellerna i målområdet. |
| [SetKeepOldTables](./setkeepoldtables/) | Behåller tabellerna i målområdet. |
| [GetOnlyVisibleCells](./getonlyvisiblecells/) | Sant betyder att endast synliga celler kopieras. |
| [SetOnlyVisibleCells](./setonlyvisiblecells/) | Sant betyder att endast synliga celler kopieras. |
| [GetTranspose](./gettranspose/) | Sant för att transponera rader och kolumner när området klistras in. Standardvärdet är Falskt. |
| [SetTranspose](./settranspose/) | Sant för att transponera rader och kolumner när området klistras in. Standardvärdet är Falskt. |
| [GetOperationType](./getoperationtype/) | Hämtar och anger operationstypen när ett område klistras in. |
| [SetOperationType](./setoperationtype/) | Hämtar och anger operationstypen när ett område klistras in. |
| [GetIgnoreLinksToOriginalFile](./getignorelinkstooriginalfile/) | Ignorera länkar till originalfilen. |
| [SetIgnoreLinksToOriginalFile](./setignorelinkstooriginalfile/) | Ignorera länkar till originalfilen. |
