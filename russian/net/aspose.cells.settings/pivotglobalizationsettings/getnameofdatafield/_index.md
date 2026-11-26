---
title: "PivotGlobalizationSettings.GetNameOfDataField"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotGlobalizationSettings. Получает отображаемое имя поля данных сводки. Формат по умолчанию — Sum Of Field"
type: docs
url: /ru/net/aspose.cells.settings/pivotglobalizationsettings/getnameofdatafield/
---
## PivotGlobalizationSettings.GetNameOfDataField method

Получает отображаемое имя поля данных сводной таблицы. Формат по умолчанию — "Sum Of Field".

```csharp
public virtual string GetNameOfDataField(ConsolidationFunction function, string name)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| функция | ConsolidationFunction | Функция используется для суммирования значений поля сводки. |
| name | String | Исходное имя поля сводки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Settings;
    using System;

    public class PivotGlobalizationSettingsMethodGetNameOfDataFieldWithConsolidationFuStringDemo
    {
        public static void Run()
        {
            try
            {
                // Создайте экземпляр PivotGlobalizationSettings
                PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

                // Определите параметры для метода GetNameOfDataField
                ConsolidationFunction function = ConsolidationFunction.Sum;
                string fieldName = "Sales";

                // Вызовите метод GetNameOfDataField
                string result = globalizationSettings.GetNameOfDataField(function, fieldName);

                // Вывести результат.
                Console.WriteLine($"Localized name for data field '{fieldName}' with function '{function}': {result}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetNameOfDataField: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [ConsolidationFunction](../../../aspose.cells/consolidationfunction/)
* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


