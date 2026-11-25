---
title: "AbstractCalculationMonitor.BeforeCalculate"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo AbstractCalculationMonitor. Implementa questo metodo per eseguire operazioni prima di calcolare una cella"
type: docs
url: /it/net/aspose.cells/abstractcalculationmonitor/beforecalculate/
---
## AbstractCalculationMonitor.BeforeCalculate method

Implementa questo metodo per eseguire operazioni prima di calcolare una cella.

```csharp
public virtual void BeforeCalculate(int sheetIndex, int rowIndex, int colIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetIndex | Int32 | Indice del foglio a cui appartiene la cella. |
| rowIndex | Int32 | Indice di riga della cella |
| colIndex | Int32 | Indice di colonna della cella |

### Osservazioni

Per le celle nelle formule di matrice, questo metodo potrebbe non essere eseguito perché generalmente quelle celle vengono calcolate insieme.

### Vedi anche

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


