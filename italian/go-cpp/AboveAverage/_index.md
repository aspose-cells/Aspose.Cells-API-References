---
title: "Classe AboveAverage"
linktitle: "AboveAverage"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe AboveAverage. Incapsula l'oggetto che rappresenta aboveaverage in Go."
type: docs
weight: 200
url: /it/go-cpp/aboveaverage/
---

## AboveAverage class

Descrivi la regola di formattazione condizionale AboveAverage. Questa regola di formattazione condizionale evidenzia le celle che sono al di sopra o al di sotto della media per tutti i valori nell'intervallo.

```go

type AboveAverage struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewAboveAverage](./newaboveaverage/) | Costruttore predefinito. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [IsAboveAverage](./isaboveaverage/) | Ottieni o imposta il flag che indica se la regola è una regola "above average". 'true' indica "above average". Il valore predefinito è true. |
| [SetIsAboveAverage](./setisaboveaverage/) | Ottieni o imposta il flag che indica se la regola è una regola "above average". 'true' indica "above average". Il valore predefinito è true. |
| [IsEqualAverage](./isequalaverage/) | Ottieni o imposta il flag che indica se i criteri 'aboveAverage' e 'belowAverage' sono inclusivi del valore medio stesso, o esclusivi di quel valore. 'true' indica di includere il valore medio nei criteri. Il valore predefinito è false. |
| [SetIsEqualAverage](./setisequalaverage/) | Ottieni o imposta il flag che indica se i criteri 'aboveAverage' e 'belowAverage' sono inclusivi del valore medio stesso, o esclusivi di quel valore. 'true' indica di includere il valore medio nei criteri. Il valore predefinito è false. |
| [GetStdDev](./getstddev/) | Ottieni o imposta il numero di deviazioni standard da includere sopra o sotto la media nella regola di formattazione condizionale. Il valore di input deve essere compreso tra 0 e 3 (inclusi 0 e 3). Impostare questo valore a 0 significa che stdDev non è impostato. Il valore predefinito è 0. |
| [SetStdDev](./setstddev/) | Ottieni o imposta il numero di deviazioni standard da includere sopra o sotto la media nella regola di formattazione condizionale. Il valore di input deve essere compreso tra 0 e 3 (inclusi 0 e 3). Impostare questo valore a 0 significa che stdDev non è impostato. Il valore predefinito è 0. |
