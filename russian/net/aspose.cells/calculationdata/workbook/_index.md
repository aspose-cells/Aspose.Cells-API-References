---
title: "CalculationData.Workbook"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CalculationData. Возвращает объект Workbook, где находится функция"
type: docs
url: /ru/net/aspose.cells/calculationdata/workbook/
---
## CalculationData.Workbook property

Получает объект Workbook, где находится функция.

```csharp
public Workbook Workbook { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyWorkbookDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте пример данных и формулу
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].Formula = "=CUSTOMFUNC()";

            // Создать параметры расчёта и зарегистрировать пользовательский движок расчёта
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new CustomCalcEngine();

            // Запустить расчёт с параметрами, чтобы продемонстрировать использование свойства Workbook
            workbook.CalculateFormula(options);

            // Отобразить результат расчёта
            Console.WriteLine("Calculated value in B1: " + worksheet.Cells["B1"].Value);
            Console.WriteLine("Modified value in C1: " + worksheet.Cells["C1"].Value);

            // Сохранить результат
            workbook.Save("PropertyWorkbookDemo.xlsx");
        }

        private class CustomCalcEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                if (data.FunctionName == "CUSTOMFUNC")
                {
                    // Получить доступ к свойству Workbook из CalculationData
                    Workbook currentWorkbook = data.Workbook;
                    Worksheet currentSheet = currentWorkbook.Worksheets[0];

                    // Продемонстрировать использование workbook для манипуляции данными
                    double inputValue = (double)currentSheet.Cells["A1"].Value;
                    currentSheet.Cells["C1"].PutValue(inputValue * 2);

                    // Установить рассчитанный результат
                    data.CalculatedValue = inputValue * 3;
                }
            }
        }
    }
}
```

### См. также

* class [Workbook](../../workbook/)
* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


