---
title: "Clase AboveAverage"
linktitle: "AboveAverage"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase AboveAverage. Encapsula el objeto que representa aboveaverage en Go."
type: docs
weight: 200
url: /es/go-cpp/aboveaverage/
---

## AboveAverage class

Describe the AboveAverage conditional formatting rule.This conditional formatting rule highlights cells thatare above or below the average for all values in the range.

```go

type AboveAverage struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
| [NewAboveAverage](./newaboveaverage/) | Default constructor. |

## Methods

| Method | Description |
| --- | --- |
| [IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
| [IsAboveAverage](./isaboveaverage/) | Obtenga o establezca la bandera que indica si la regla es una regla de "promedio superior". 'true' indica 'promedio superior'. El valor predeterminado es true. |
| [SetIsAboveAverage](./setisaboveaverage/) | Obtenga o establezca la bandera que indica si la regla es una regla de "promedio superior". 'true' indica 'promedio superior'. El valor predeterminado es true. |
| [IsEqualAverage](./isequalaverage/) | Obtenga o establezca la bandera que indica si los criterios 'aboveAverage' y 'belowAverage' son inclusivos del promedio mismo, o exclusivos de ese valor. 'true' indica incluir el valor promedio en los criterios. El valor predeterminado es false. |
| [SetIsEqualAverage](./setisequalaverage/) | Obtenga o establezca la bandera que indica si los criterios 'aboveAverage' y 'belowAverage' son inclusivos del promedio mismo, o exclusivos de ese valor. 'true' indica incluir el valor promedio en los criterios. El valor predeterminado es false. |
| [GetStdDev](./getstddev/) | Obtenga o establezca el número de desviaciones estándar para incluir por encima o por debajo del promedio en la regla de formato condicional. El valor de entrada debe estar entre 0 y 3 (incluyendo 0 y 3). Establecer este valor en 0 significa que stdDev no está configurado. El valor predeterminado es 0. |
| [SetStdDev](./setstddev/) | Obtenga o establezca el número de desviaciones estándar para incluir por encima o por debajo del promedio en la regla de formato condicional. El valor de entrada debe estar entre 0 y 3 (incluyendo 0 y 3). Establecer este valor en 0 significa que stdDev no está configurado. El valor predeterminado es 0. |
