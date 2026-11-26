---
title: "Перечисление CalcModeType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.CalcModeType. Представляет тип режима вычисления формул"
type: docs
url: /ru/net/aspose.cells/calcmodetype/
---
## CalcModeType enumeration

Представляет тип режима вычисления формул.

```csharp
public enum CalcModeType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Automatic | `0` |  |
| AutomaticExceptTable | `1` |  |
| Manual | `2` |  |

### Примечания

Только для MS Excel.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalcModeTypeDemo
    {
        public static void CalcModeTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для теста
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["B2"].PutValue(3);
            worksheet.Cells["B3"].PutValue(4);
            worksheet.Cells["C1"].PutValue(5);
            worksheet.Cells["C2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(15);

            worksheet.Cells["A4"].Formula = "=A1+B1+C1";
            worksheet.Cells["B4"].Formula = "=SUM(B1:B3)";

            // Получите доступ к настройкам формул книги
            FormulaSettings formulaSettings = workbook.Settings.FormulaSettings;

            // Установите режим вычисления в Manual
            formulaSettings.CalculationMode = CalcModeType.Manual;

            // Установите другие настройки формул
            formulaSettings.CalculateOnOpen = true;
            formulaSettings.CalculateOnSave = true;
            formulaSettings.ForceFullCalculation = false;
            formulaSettings.CalculationId = "0";
            formulaSettings.EnableIterativeCalculation = true;
            formulaSettings.MaxIteration = 100;
            formulaSettings.MaxChange = 0.001;
            formulaSettings.PrecisionAsDisplayed = false;
            formulaSettings.EnableCalculationChain = true;
            formulaSettings.PreservePaddingSpaces = false;

            // Сохраните книгу
            workbook.Save("CalcModeTypeExample.xlsx");
            workbook.Save("CalcModeTypeExample.pdf");

        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


