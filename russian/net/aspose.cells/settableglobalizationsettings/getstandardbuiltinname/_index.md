---
title: "SettableGlobalizationSettings.GetStandardBuiltInName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableGlobalizationSettings. Получает стандартный текст встроенного имени в соответствии с заданным текстом, зависящим от локали"
type: docs
url: /ru/net/aspose.cells/settableglobalizationsettings/getstandardbuiltinname/
---
## SettableGlobalizationSettings.GetStandardBuiltInName method

Получает стандартный текст встроенного имени в соответствии с заданным текстом, зависящим от локали.

```csharp
public override string GetStandardBuiltInName(string localName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| localName | String | Текст встроенного имени, зависящий от локали. Локаль была указана книгой Excel, для которой используются эти настройки. |

### Возвращаемое значение

Стандартный текст (локаль en-US).

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetStandardBuiltInNameWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте экземпляр SettableGlobalizationSettings
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

            // Установите локальное встроенное имя для демонстрации
            globalizationSettings.SetLocalBuiltInName("SUM", "LocalSumName", true);

            try
            {
                // Вызовите метод GetStandardBuiltInName с локальным именем
                string standardName = globalizationSettings.GetStandardBuiltInName("LocalSumName");
                
                // Отобразить результат
                Console.WriteLine($"Standard name for 'LocalSumName' is: {standardName}");

                // Примените результат к ячейке
                worksheet.Cells["A1"].Formula = "=" + standardName + "(1,2,3)";
                workbook.CalculateFormula();

                // Отобразите вычисленный результат
                Console.WriteLine($"Result of formula in A1: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardBuiltInName method: {ex.Message}");
            }
            
            // Сохраните книгу
            workbook.Save("SettableGlobalizationSettingsMethodGetStandardBuiltInNameWithStringDemo.xlsx");
        }
    }
}
```

### См. также

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


