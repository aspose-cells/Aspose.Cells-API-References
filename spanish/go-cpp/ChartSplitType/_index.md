---
title: "Enumeración ChartSplitType"
linktitle: "ChartSplitType"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Enumeración ChartSplitType. Encapsula el objeto que representa chartsplittype en Go."
type: docs
weight: 200
url: /es/go-cpp/chartsplittype/
---

## ChartSplitType Enum

Represents the way the two sections of either a pie of pie chart or a bar of pie chart are split.

```go

type ChartSplitType int32


```

## Fields

| Field | Description |
| --- | --- |
| [Position](./position/) | Representa los puntos de datos. Los puntos de datos se dividirán entre el gráfico de pastel y el segundo gráfico colocando la última posición de división de los puntos de datos en el segundo gráfico. |
| [Value](./value/) | Representa los puntos de datos que se dividirán entre el gráfico de pastel y el segundo gráfico colocando los puntos de datos con valor inferior a Split Position en el segundo gráfico. |
| [PercentValue](./percentvalue/) | Representa los puntos de datos que se dividirán entre el gráfico de pastel y el segundo gráfico colocando los puntos con un porcentaje inferior al porcentaje Split Position en el segundo gráfico. |
| [Custom](./custom/) | Representa los puntos de datos que se dividirán entre el gráfico de pastel y el segundo gráfico según los valores de división personalizados. |
| [Auto](./auto/) | Representa los puntos de datos que se dividirán utilizando el mecanismo predeterminado para este tipo de gráfico. |
