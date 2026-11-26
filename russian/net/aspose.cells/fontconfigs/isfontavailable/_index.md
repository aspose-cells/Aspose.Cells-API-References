---
title: "FontConfigs.IsFontAvailable"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод FontConfigs. Указывает, доступен ли шрифт"
type: docs
url: /ru/net/aspose.cells/fontconfigs/isfontavailable/
---
## FontConfigs.IsFontAvailable method

Указывает, доступен ли шрифт.

```csharp
public static bool IsFontAvailable(string fontName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fontName | String | название шрифта |

### Возвращаемое значение

true, если шрифт доступен, иначе false.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsMethodIsFontAvailableWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Проверьте имена шрифтов, чтобы проверить их доступность
            string[] testFonts = { "Arial", "Times New Roman", "NonExistentFont" };

            try
            {
                foreach (string fontName in testFonts)
                {
                    // Вызовите метод IsFontAvailable с именем шрифта
                    bool isAvailable = FontConfigs.IsFontAvailable(fontName);

                    // Отобразить результат
                    Console.WriteLine($"Font '{fontName}' is available: {isAvailable}");

                    // Записать результат в лист
                    int row = worksheet.Cells.MaxDataRow + 1;
                    worksheet.Cells[row, 0].PutValue($"Font '{fontName}' available:");
                    worksheet.Cells[row, 1].PutValue(isAvailable);
                }

                Console.WriteLine("Method executed successfully with parameters (String)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsFontAvailable method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("FontConfigsMethodIsFontAvailableWithStringDemo.xlsx");
        }
    }
}
```

### См. также

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


