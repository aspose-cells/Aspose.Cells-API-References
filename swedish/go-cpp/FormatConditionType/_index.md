---
title: "FormatConditionType enum"
linktitle: "FormatConditionType"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "FormatConditionType-enum. Inkapslar objektet som representerar formatconditiontype i Go."
type: docs
weight: 200
url: /sv/go-cpp/formatconditiontype/
---

## FormatConditionType Enum

Typ av villkorsformatregel.

```go

type FormatConditionType int32


```

## Fält

| Fält | Beskrivning |
| --- | --- |
| [CellValue](./cellvalue/) | Denna villkorsformateringsregel jämför ett cellvärde med ett formelberäknat resultat, med hjälp av en operator. |
| [Expression](./expression/) | Denna villkorsformateringsregel innehåller en formel att utvärdera. När formelresultatet är sant, markeras cellen. |
| [Top10](./top10/) | Denna villkorsformateringsregel markerar celler vars värden faller inom den översta N eller nedersta N intervallen, enligt specifikation. |
| [UniqueValues](./uniquevalues/) | Denna villkorsformateringsregel markerar unika värden i intervallet. |
| [DuplicateValues](./duplicatevalues/) | Denna villkorsformateringsregel markerar duplicerade värden. |
| [ContainsText](./containstext/) | Denna villkorsformateringsregel markerar celler som innehåller given text. Motsvarande att använda SEARCH()-bladfunktionen för att avgöra om cellen innehåller texten. |
| [NotContainsText](./notcontainstext/) | Denna villkorsformateringsregel markerar celler som inte innehåller given text. Motsvarande att använda SEARCH()-bladfunktionen för att avgöra om cellen innehåller texten eller inte. |
| [BeginsWith](./beginswith/) | Denna villkorsformateringsregel markerar celler i intervallet som börjar med den givna texten. Motsvarande att använda LEFT()-bladfunktionen och jämföra värden. |
| [EndsWith](./endswith/) | Denna villkorsformateringsregel markerar celler som slutar med given text. Motsvarande att använda RIGHT()-bladfunktionen och jämföra värden. |
| [ContainsBlanks](./containsblanks/) | Denna villkorsformateringsregel markerar celler som är helt tomma. Motsvarande att använda LEN(TRIM()). Detta betyder att om cellen bara innehåller tecken som TRIM() skulle ta bort, anses den vara tom. En tom cell anses också vara tom. |
| [NotContainsBlanks](./notcontainsblanks/) | Denna villkorsformateringsregel markerar celler som inte är tomma. Motsvarande att använda LEN(TRIM()). Detta betyder att om cellen bara innehåller tecken som TRIM() skulle ta bort, anses den vara tom. En tom cell anses också vara tom. |
| [ContainsErrors](./containserrors/) | Denna villkorsformateringsregel markerar celler med formelfel. Motsvarande att använda ISERROR() bladfunktion för att avgöra om det finns ett formelfel. |
| [NotContainsErrors](./notcontainserrors/) | Denna villkorsformateringsregel markerar celler utan formelfel. Motsvarande att använda ISERROR() bladfunktion för att avgöra om det finns ett formelfel. |
| [TimePeriod](./timeperiod/) | Denna villkorsformateringsregel markerar celler som innehåller datum inom den angivna tidsperioden. Cellens underliggande värde utvärderas, så cellen behöver inte vara formaterad som ett datum för att utvärderas. Till exempel, med en cell som innehåller värdet 38913 ska det villkorliga formatet tillämpas om regeln kräver ett värde av 14/7/2006. |
| [AboveAverage](./aboveaverage/) | Denna villkorsformateringsregel markerar celler som är över eller under genomsnittet för alla värden i intervallet. |
| [ColorScale](./colorscale/) | Denna villkorsformateringsregel skapar en graderad färgskala på cellerna. |
| [DataBar](./databar/) | Denna villkorsformateringsregel visar en graderad datastapel i cellintervallet. |
| [IconSet](./iconset/) | Denna villkorsformateringsregel tillämpar ikoner på celler enligt deras värden. |
