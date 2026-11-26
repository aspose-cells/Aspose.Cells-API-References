---
title: "AbstractCalculationMonitor.BeforeCalculate"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método AbstractCalculationMonitor. Implementa este método para realizar operaciones antes de calcular una celda"
type: docs
url: /es/net/aspose.cells/abstractcalculationmonitor/beforecalculate/
---
## AbstractCalculationMonitor.BeforeCalculate method

Implementa este método para realizar acciones antes de calcular una celda.

```csharp
public virtual void BeforeCalculate(int sheetIndex, int rowIndex, int colIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetIndex | Int32 | Índice de la hoja a la que pertenece la celda. |
| rowIndex | Int32 | Índice de fila de la celda |
| colIndex | Int32 | Índice de columna de la celda |

### Observaciones

Para celdas en fórmulas de matriz, este método puede no ejecutarse porque generalmente esas celdas se calculan juntas.

### Ver también

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


