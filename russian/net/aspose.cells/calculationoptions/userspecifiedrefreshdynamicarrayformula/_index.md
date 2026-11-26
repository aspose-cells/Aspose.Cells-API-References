---
title: "CalculationOptions.UserSpecifiedRefreshDynamicArrayFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CalculationOptions. Указывает, явно ли пользователь задал поведение обновления динамических массивных формул перед вычислением указанных формул"
type: docs
url: /ru/net/aspose.cells/calculationoptions/userspecifiedrefreshdynamicarrayformula/
---
## CalculationOptions.UserSpecifiedRefreshDynamicArrayFormula property

Указывает, указал ли пользователь явно поведение обновления формул динамических массивов перед вычислением указанных формул.

```csharp
public bool UserSpecifiedRefreshDynamicArrayFormula { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationOptionsPropertyUserSpecifiedRefreshDynamicArrayFormulaDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Создайте пример рабочего листа
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые данные, чтобы пример имел смысл
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Создайте экземпляр CalculationOptions
                CalculationOptions options = new CalculationOptions();

                // Отобразить текущее значение свойства UserSpecifiedRefreshDynamicArrayFormula
                Console.WriteLine("UserSpecifiedRefreshDynamicArrayFormula value: " +
                    options.UserSpecifiedRefreshDynamicArrayFormula);

                // Показать, как свойство влияет на поведение
                Console.WriteLine("UserSpecifiedRefreshDynamicArrayFormula has been demonstrated");

                // Сохранить результат
                workbook.Save("UserSpecifiedRefreshDynamicArrayFormulaDemo.xlsx");
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


