---
title: AbstractCalculationMonitor
second_title: Справочник по Aspose.Cells для .NET API
description: Монитор для отслеживания пользователем хода вычисления формулы.
type: docs
weight: 30
url: /ru/net/aspose.cells/abstractcalculationmonitor/
---
## AbstractCalculationMonitor class

Монитор для отслеживания пользователем хода вычисления формулы.

```csharp
public abstract class AbstractCalculationMonitor
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [CalculatedValue](../../aspose.cells/abstractcalculationmonitor/calculatedvalue) { get; } | Получает новое вычисленное значение ячейки. Следует использовать только в[`AfterCalculate`](./aftercalculate). |
| [OriginalValue](../../aspose.cells/abstractcalculationmonitor/originalvalue) { get; } | Получает старое значение вычисляемой ячейки. Следует использовать только в[`BeforeCalculate`](./beforecalculate)и[`AfterCalculate`](./aftercalculate). |
| [ValueChanged](../../aspose.cells/abstractcalculationmonitor/valuechanged) { get; } | Изменилось ли значение ячейки после вычисления. Следует использовать только в[`AfterCalculate`](./aftercalculate). |

## Методы

| Имя | Описание |
| --- | --- |
| virtual [AfterCalculate](../../aspose.cells/abstractcalculationmonitor/aftercalculate)(int, int, int) | Реализуйте этот метод для ведения бизнеса после расчета одной ячейки. |
| virtual [BeforeCalculate](../../aspose.cells/abstractcalculationmonitor/beforecalculate)(int, int, int) | Реализуйте этот метод, чтобы вести дела перед вычислением одной ячейки. |
| virtual [OnCircular](../../aspose.cells/abstractcalculationmonitor/oncircular)(IEnumerator) | Реализуйте этот метод для ведения бизнеса при расчете формул с циклическими ссылками. |

### Примеры

```csharp
[C#]
  //Пользовательский монитор для проверки возможности StackOverflowException
public class MyCalculationMonitor : AbstractCalculationMonitor
{
    public override void BeforeCalculate(int sheetIndex, int rowIndex, int colIndex)
    {
        if(new StackTrace(false).FrameCount > 1000)
        {
            throw new Exception("Stop the formula calculation because risk of StackOverflowException");
        }
    }
}
```

### Смотрите также

* пространство имен [Aspose.Cells](../../aspose.cells)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
