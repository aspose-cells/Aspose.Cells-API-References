---
title: "ChartSplitType Enum"
linktitle: "ChartSplitType"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "ChartSplitType enum. Incapsula l'oggetto che rappresenta chartsplittype in Go."
type: docs
weight: 200
url: /it/go-cpp/chartsplittype/
---

## ChartSplitType Enum

Rappresenta il modo in cui le due sezioni di un grafico a torta di torta o a barra di torta sono suddivise.

```go

type ChartSplitType int32


```

## Campi

| Campo | Descrizione |
| --- | --- |
| [Position](./position/) | Rappresenta i punti dati.I punti dati devono essere suddivisi tra il grafico a torta e il secondo grafico posizionando l'ultima posizione di divisione dei punti dati nel secondo grafico. |
| [Value](./value/) | Rappresenta i punti dati devono essere suddivisi tra il pieand e il secondo grafico posizionando i punti dati convalue inferiore a Split Position nel secondo grafico. |
| [PercentValue](./percentvalue/) | Rappresenta i punti dati che devono essere suddivisi tra il grafico a torta e il secondo grafico posizionando i punti con una percentuale inferiore al percento Split Position nel secondo grafico. |
| [Custom](./custom/) | Rappresenta i punti dati devono essere suddivisi tra il pieand e il secondo grafico secondo i Custom Splitvalues. |
| [Auto](./auto/) | Rappresenta i punti dati che devono essere suddivisi utilizzando il meccanismo predefinito per questo tipo di grafico. |
