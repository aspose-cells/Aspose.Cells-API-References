---
title: "CellsHelper.SignificantDigitsType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CellsHelper. Получает и задает тип значимых цифр по умолчанию для вывода числовых значений. Значение по умолчанию — G17"
type: docs
url: /ru/net/aspose.cells/cellshelper/significantdigitstype/
---
## CellsHelper.SignificantDigitsType property

Получает и задает тип значимых цифр по умолчанию для вывода числовых значений. Значение по умолчанию — G17.

```csharp
public static SignificantDigitsType SignificantDigitsType { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperPropertySignificantDigitsTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Отобразить текущее значение SignificantDigitsType
                Console.WriteLine("Current SignificantDigitsType: " + CellsHelper.SignificantDigitsType);

                // Установить новое значение SignificantDigitsType
                CellsHelper.SignificantDigitsType = SignificantDigitsType.G17;
                Console.WriteLine("Updated SignificantDigitsType: " + CellsHelper.SignificantDigitsType);

                // Создать книгу для демонстрации эффекта
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Добавить числовое значение, которое будет обрабатываться с учётом значимых цифр
                worksheet.Cells["A1"].PutValue(1.2345678912345678);
                worksheet.Cells["A2"].PutValue(1.2345678912345678);
                worksheet.Cells["A3"].Formula = "=A1+A2";

                // Вычислить формулы с текущим типом значимых цифр
                workbook.CalculateFormula();

                // Отобразить результат
                Console.WriteLine("Calculation result: " + worksheet.Cells["A3"].Value);

                // Переключить на другой тип значимых цифр
                CellsHelper.SignificantDigitsType = SignificantDigitsType.Rounding17;
                Console.WriteLine("Changed SignificantDigitsType: " + CellsHelper.SignificantDigitsType);

                // Пересчитать с новым типом значимых цифр
                workbook.CalculateFormula();
                Console.WriteLine("Recalculated result: " + worksheet.Cells["A3"].Value);

                // Сохраните книгу
                workbook.Save("SignificantDigitsTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [SignificantDigitsType](../../significantdigitstype/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


