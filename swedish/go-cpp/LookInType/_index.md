---
title: "LookInType-enum"
linktitle: "LookInType"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "LookInType-enum. Inkapslar objektet som representerar lookintype i Go."
type: docs
weight: 200
url: /sv/go-cpp/lookintype/
---

## LookInType Enum

Representerar typ av 'look in'.

```go

type LookInType int32


```

## Fält

| Fält | Beskrivning |
| --- | --- |
| [Formulas](./formulas/) | Hittar det sökta objektet från formeln(<see cref=\"Cell.Formula\"/>) om cellen är en formel, annars hittas det från cellens ursprungliga värde (samma som <see cref=\"OriginalValues\"/>). |
| [Values](./values/) | Hittar objektet från cellens ursprungliga värde(<see cref=\"Cell.Value\"/>) och det formaterade värdet(<see cref=\"Cell.StringValue\"/>). |
| [ValuesExcludeFormulaCell](./valuesexcludeformulacell/) | Ignorerar celler som är formler. För de celler som inte är formler är det samma som <see cref=\"Values\"/>. |
| [Comments](./comments/) | Hittar objektet endast från cellens kommentar. Ignorerar de celler som saknar kommentar. |
| [OnlyFormulas](./onlyformulas/) | Ignorerar celler som inte är formler. För de celler som är förmler hittas det sökta objektet från formeln(<see cref=\"Cell.Formula\"/>). |
| [OriginalValues](./originalvalues/) | Hitta objektet endast från cellens ursprungliga värde. |
| [FormattedValues](./formattedvalues/) | Hitta objektet endast från cellens formaterade värde(<see cref=\"Cell.StringValue\"/>). |
