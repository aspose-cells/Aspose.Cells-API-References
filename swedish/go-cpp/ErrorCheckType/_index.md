---
title: "ErrorCheckType‑enum"
linktitle: "ErrorCheckType"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "ErrorCheckType‑enum. Inkapslar objektet som representerar errorchecktype i Go."
type: docs
weight: 200
url: /sv/go-cpp/errorchecktype/
---

## ErrorCheckType Enum

Representerar alla felkontrolltyper.

```go

type ErrorCheckType int32


```

## Fält

| Fält | Beskrivning |
| --- | --- |
| [EvaluationError](./evaluationerror/) | Ignorera fel när celler innehåller formler som resulterar i ett fel. |
| [EmptyCellRef](./emptycellref/) | Ignorera fel när formler refererar till tomma celler. |
| [NumberStoredAsText](./numberstoredastext/) | Ignorera fel när tal är formaterade som text eller föregås av ett apostrof |
| [InconsistRange](./inconsistrange/) | Ignorera fel när formler utelämnar vissa celler i ett område. |
| [InconsistFormula](./inconsistformula/) | Ignorera fel när en formel i ett område i ditt kalkylblad skiljer sig från andra formler i samma område. |
| [TwoDigitTextYear](./twodigittextyear/) | Ignorera fel när formler innehåller textformaterade celler med år representerade med två siffror. |
| [UnlockedFormula](./unlockedformula/) | Ignorera fel när olåsta celler innehåller formler. |
| [TableDataValidation](./tabledatavalidation/) | Ignorera fel när en cells värde i en tabell inte följer de angivna datavalideringsreglerna. |
| [CalculatedColumn](./calculatedcolumn/) | Ignorera fel när celler innehåller ett värde som skiljer sig från en beräknad kolumnformel. |
