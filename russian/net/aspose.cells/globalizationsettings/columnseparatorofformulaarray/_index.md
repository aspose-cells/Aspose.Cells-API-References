---
title: "GlobalizationSettings.ColumnSeparatorOfFormulaArray"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство GlobalizationSettings. Получает разделитель элементов в массиве данных строк формулы"
type: docs
url: /ru/net/aspose.cells/globalizationsettings/columnseparatorofformulaarray/
---
## GlobalizationSettings.ColumnSeparatorOfFormulaArray property

Получает разделитель для элементов в строковых данных массива в формуле.

```csharp
public virtual char ColumnSeparatorOfFormulaArray { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsPropertyColumnSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать пользовательские параметры глобализации с переопределённым разделителем столбцов
            var globalizationSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = globalizationSettings;

            // Отобразить текущее значение разделителя столбцов
            Console.WriteLine("Current ColumnSeparatorOfFormulaArray value: " +
                globalizationSettings.ColumnSeparatorOfFormulaArray);

            // Создать массивную формулу, используя пользовательский разделитель
            Cell cell = worksheet.Cells["A1"];
            cell.SetArrayFormula("=SUM({1;2;3;4})", 1, 1); // Uses custom ';' column separator

            // Проверить хранение формулы (в реальной строке формулы будут показаны точки с запятой)
            Console.WriteLine("Stored array formula: " + cell.Formula);

            // Сохранить изменённую книгу
            workbook.Save("PropertyColumnSeparatorOfFormulaArrayDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override char ColumnSeparatorOfFormulaArray => ';';
        }
    }
}
```

### См. также

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


