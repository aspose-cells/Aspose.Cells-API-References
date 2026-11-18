---
title: "DeleteBlankOptions-klass"
linktitle: "DeleteBlankOptions"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "DeleteBlankOptions-klass. Inkapslar objektet som representerar deleteblankoptions i Go."
type: docs
weight: 200
url: /sv/go-cpp/deleteblankoptions/
---

## DeleteBlankOptions class

Representerar inställningen för att ta bort tomma celler/rader/kolumner.

```go

type DeleteBlankOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewDeleteBlankOptions](./newdeleteblankoptions/) | Standardkonstruktor. |
| [NewDeleteBlankOptions_DeleteOptions](./newdeleteblankoptions_deleteoptions/) | Skapas från ett föräldraobjekt. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetEmptyStringAsBlank](./getemptystringasblank/) | Indikerar om en cell ska betraktas som tom när dess värde är en tom sträng. Standardvärdet är true. |
| [SetEmptyStringAsBlank](./setemptystringasblank/) | Indikerar om en cell ska betraktas som tom när dess värde är en tom sträng. Standardvärdet är true. |
| [GetEmptyFormulaValueAsBlank](./getemptyformulavalueasblank/) | Om en cell ska betraktas som tom när den är en formel och det beräknade resultatet är null eller en tom sträng. Standardvärdet är false. |
| [SetEmptyFormulaValueAsBlank](./setemptyformulavalueasblank/) | Om en cell ska betraktas som tom när den är en formel och det beräknade resultatet är null eller en tom sträng. Standardvärdet är false. |
| [GetDrawingsAsBlank](./getdrawingsasblank/) | Indikerar om ritningsrelaterade objekt såsom bild, form, diagram... ska betraktas som tomma. Standardvärdet är true. |
| [SetDrawingsAsBlank](./setdrawingsasblank/) | Indikerar om ritningsrelaterade objekt såsom bild, form, diagram... ska betraktas som tomma. Standardvärdet är true. |
| [GetMergedCellsShrinkType](./getmergedcellsshrinktype/) | Indikerar hur sammanslagna celler ska behandlas vid borttagning av tomma rader/kolumner. |
| [SetMergedCellsShrinkType](./setmergedcellsshrinktype/) | Indikerar hur sammanslagna celler ska behandlas vid borttagning av tomma rader/kolumner. |
| [GetStartIndex](./getstartindex/) | Anger startrad-/kolumnindex för området som ska kontrolleras och där tomma rader/kolumner ska tas bort. |
| [SetStartIndex](./setstartindex/) | Anger startrad-/kolumnindex för området som ska kontrolleras och där tomma rader/kolumner ska tas bort. |
| [GetEndIndex](./getendindex/) | Anger slutrad-/kolumnindex (inklusive) för området som ska kontrolleras och där tomma rader/kolumner ska tas bort. Standardvärdet är -1 och -1 betyder det maximala området för alla objekt (celler, ritningar, ...) som måste kontrolleras. |
| [SetEndIndex](./setendindex/) | Anger slutrad-/kolumnindex (inklusive) för området som ska kontrolleras och där tomma rader/kolumner ska tas bort. Standardvärdet är -1 och -1 betyder det maximala området för alla objekt (celler, ritningar, ...) som måste kontrolleras. |
| [GetUpdateReference](./getupdatereference/) | Anger om uppdateringsreferenser i andra kalkylblad. |
| [SetUpdateReference](./setupdatereference/) | Anger om uppdateringsreferenser i andra kalkylblad. |
| [GetFormulaChangeMonitor](./getformulachangemonitor/) | Hämtar/anger övervakaren för att spåra förändringar som orsakas av borttagningen. |
| [SetFormulaChangeMonitor](./setformulachangemonitor/) | Hämtar/anger övervakaren för att spåra förändringar som orsakas av borttagningen. |
