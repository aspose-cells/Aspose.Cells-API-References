---
title: "CalculationData.ParamCount"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CalculationData. Возвращает количество параметров"
type: docs
url: /ru/net/aspose.cells/calculationdata/paramcount/
---
## CalculationData.ParamCount property

Получает количество параметров

```csharp
public int ParamCount { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyParamCountDemo
    {
        public static void Run()
        {
            try
            {
                // Создайте новую книгу и получите первый лист
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Заполнить несколько ячеек, которые будут использоваться в качестве параметров
                sheet.Cells["A1"].PutValue(10);
                sheet.Cells["A2"].PutValue(20);
                sheet.Cells["A3"].PutValue(30);

                // Установить формулу, вызывающую пользовательскую функцию с тремя аргументами
                sheet.Cells["B1"].Formula = "=DEMOPARAM(A1, A2, A3)";

                // Настройте параметры вычисления для использования пользовательского движка
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new ParamCountEngine();

                // Выполнить вычисление
                workbook.CalculateFormula(options);

                // Пользовательский движок возвращает ParamCount как вычисленное значение
                Console.WriteLine("ParamCount reported by custom function: " + sheet.Cells["B1"].Value);
                
                // Опционально сохранить книгу
                workbook.Save("ParamCountDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        // Пользовательский вычислительный движок, демонстрирующий чтение свойства ParamCount
        private class ParamCountEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                // Определить пользовательскую функцию по имени
                if (data.FunctionName != null && data.FunctionName.Equals("DEMOPARAM", StringComparison.OrdinalIgnoreCase))
                {
                    // Прочитать только‑для‑чтения свойство ParamCount
                    int count = data.ParamCount;

                    // Использовать количество в качестве результата функции
                    data.CalculatedValue = count;
                }
            }
        }
    }
}
```

### См. также

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


