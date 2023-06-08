---
title: Class AbstractCalculationMonitor
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.AbstractCalculationMonitor class. Monitor for user to track the progress of formula calculation
type: docs
url: /net/aspose.cells/abstractcalculationmonitor/
---
## AbstractCalculationMonitor class

Monitor for user to track the progress of formula calculation.

```csharp
public abstract class AbstractCalculationMonitor
```

## Properties

| Name | Description |
| --- | --- |
| [CalculatedValue](../../aspose.cells/abstractcalculationmonitor/calculatedvalue/) { get; } | Gets the newly calculated value of the cell. Should be used only in [`AfterCalculate`](./aftercalculate/). |
| [OriginalValue](../../aspose.cells/abstractcalculationmonitor/originalvalue/) { get; } | Gets the old value of the calculated cell. Should be used only in [`BeforeCalculate`](./beforecalculate/) and [`AfterCalculate`](./aftercalculate/). |
| [ValueChanged](../../aspose.cells/abstractcalculationmonitor/valuechanged/) { get; } | Whether the cell's value has been changed after the calculation. Should be used only in [`AfterCalculate`](./aftercalculate/). |

## Methods

| Name | Description |
| --- | --- |
| virtual [AfterCalculate](../../aspose.cells/abstractcalculationmonitor/aftercalculate/)(int, int, int) | Implement this method to do business after one cell has been calculated. |
| virtual [BeforeCalculate](../../aspose.cells/abstractcalculationmonitor/beforecalculate/)(int, int, int) | Implement this method to do business before calculating one cell. |
| virtual [OnCircular](../../aspose.cells/abstractcalculationmonitor/oncircular/)(IEnumerator) | Implement this method to do business when calculating formulas with circular references. |

### Examples

```csharp
[C#]
Workbook wb = new Workbook("calc.xlsx");
CalculationOptions opts = new CalculationOptions();
opts.CalculationMonitor = new MyCalculationMonitor();
wb.CalculateFormula(opts);

class MyCalculationMonitor : AbstractCalculationMonitor
{
    public override void BeforeCalculate(int sheetIndex, int rowIndex, int colIndex)
    {
        if(sheetIndex!=0 || rowIndex!=0 || colIndex!=0)
        {
            return;
        }
        Console.WriteLine("Cell A1 will be calculated.");
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


