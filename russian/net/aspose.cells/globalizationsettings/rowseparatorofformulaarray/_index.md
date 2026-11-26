---
title: "GlobalizationSettings.RowSeparatorOfFormulaArray"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство GlobalizationSettings. Возвращает разделитель строк в массивных данных формулы"
type: docs
url: /ru/net/aspose.cells/globalizationsettings/rowseparatorofformulaarray/
---
## GlobalizationSettings.RowSeparatorOfFormulaArray property

Получает разделитель для строк в массивных данных в формуле.

```csharp
public virtual char RowSeparatorOfFormulaArray { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsPropertyRowSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // Создать новую рабочую книгу с пользовательскими настройками глобализации
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить экземпляр пользовательских настроек глобализации
            CustomGlobalizationSettings settings = (CustomGlobalizationSettings)workbook.Settings.GlobalizationSettings;

            // Отобразить текущее значение RowSeparatorOfFormulaArray
            Console.WriteLine("Current RowSeparatorOfFormulaArray value: " + settings.RowSeparatorOfFormulaArray);

            // Создать формулу массива, используя пользовательский разделитель строк
            Cell cell = worksheet.Cells["A1"];
            cell.Formula = "=SUM({1,2|3,4})"; // Uses '|' as row separator

            // Вычислить формулу, чтобы продемонстрировать правильный разбор
            workbook.CalculateFormula();

            // Отобразить результаты
            Console.WriteLine("Array formula using custom separator: " + cell.Formula);
            Console.WriteLine("Calculated result: " + cell.Value);

            // Сохраните книгу
            workbook.Save("PropertyRowSeparatorOfFormulaArrayDemo.xlsx");
        }
    }

    // Пользовательская реализация GlobalizationSettings, переопределяющая разделитель строк
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override char RowSeparatorOfFormulaArray => '|';
    }
}
```

### См. также

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


