---
title: "AbstractCalculationMonitor.BeforeCalculate"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод AbstractCalculationMonitor. Реализуйте этот метод для выполнения бизнес-логики перед вычислением одной ячейки"
type: docs
url: /ru/net/aspose.cells/abstractcalculationmonitor/beforecalculate/
---
## AbstractCalculationMonitor.BeforeCalculate method

Реализуйте этот метод для выполнения бизнес-логики перед вычислением ячейки.

```csharp
public virtual void BeforeCalculate(int sheetIndex, int rowIndex, int colIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetIndex | Int32 | Индекс листа, к которому относится ячейка. |
| rowIndex | Int32 | Индекс строки ячейки |
| colIndex | Int32 | Индекс столбца ячейки |

### Примечания

Для ячеек в массивных формулах этот метод может не быть выполнен, поскольку обычно такие ячейки рассчитываются вместе.

### См. также

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


