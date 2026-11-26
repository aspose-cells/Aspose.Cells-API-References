---
title: "CalculationOptions.RefreshDynamicArrayFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CalculationOptions. Указывает, следует ли обновлять формулы динамических массивов перед вычислением формул"
type: docs
url: /ru/net/aspose.cells/calculationoptions/refreshdynamicarrayformula/
---
## CalculationOptions.RefreshDynamicArrayFormula property

Указывает, следует ли обновлять формулы динамических массивов перед вычислением формул.

```csharp
public bool RefreshDynamicArrayFormula { get; set; }
```

### Примечания

Если это свойство указано явно, то указанное значение будет использоваться для определения необходимости обновления формул динамических массивов. В противном случае ([`UserSpecifiedRefreshDynamicArrayFormula`](../userspecifiedrefreshdynamicarrayformula/) — false), значение по умолчанию зависит от того, какие формулы необходимо вычислять: для вычисления формул книги, например [`CalculateFormula`](../../workbook/calculateformula/), это свойство считается истинным. В остальных случаях, например [`Calculate`](../../cell/calculate/) или [`CalculateFormula`](../../worksheet/calculateformula/), это свойство считается ложным.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationOptionsPropertyRefreshDynamicArrayFormulaDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте формулу динамического массива, чтобы продемонстрировать функциональность
            worksheet.Cells["A1"].Value = 1;
            worksheet.Cells["A2"].Value = 2;
            worksheet.Cells["A3"].Value = 3;
            worksheet.Cells["B1"].Formula = "=A1:A3"; // Dynamic array formula

            // Создайте экземпляр CalculationOptions
            CalculationOptions options = new CalculationOptions();

            try
            {
                // Отобразите значение по умолчанию свойства RefreshDynamicArrayFormula
                Console.WriteLine("Default RefreshDynamicArrayFormula value: " + options.RefreshDynamicArrayFormula);

                // Установите свойство в true, чтобы обновлять формулы динамических массивов
                options.RefreshDynamicArrayFormula = true;
                Console.WriteLine("After setting to true: " + options.RefreshDynamicArrayFormula);

                // Вычислите формулы с указанными параметрами
                workbook.CalculateFormula(options);

                // Отобразите вычисленный результат
                Console.WriteLine("Dynamic array formula result: " + worksheet.Cells["B1"].Value);

                // Сохраните книгу
                workbook.Save("RefreshDynamicArrayFormulaDemo.xlsx");
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

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


