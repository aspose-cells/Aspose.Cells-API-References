---
title: "SettableGlobalizationSettings.SetStandardBuiltInName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableGlobalizationSettings. Устанавливает зависящее от локали имя функции в соответствии с заданным стандартным именем функции"
type: docs
url: /ru/net/aspose.cells/settableglobalizationsettings/setstandardbuiltinname/
---
## SettableGlobalizationSettings.SetStandardBuiltInName method

Устанавливает зависящее от локали имя функции в соответствии с заданным стандартным именем функции.

```csharp
public void SetStandardBuiltInName(string localName, string standardName, bool bidirectional)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| localName | String | Зависящее от локали имя функции |
| standardName | String | Стандартное имя функции (локаль en-US). |
| bidirectional | Boolean | Нужно ли автоматически сопоставлять текст стандартного имени с текстом локального имени. Если true, текст стандартного имени будет автоматически сопоставлен с текстом локального имени, так что пользователю не нужно вызывать [`SetLocalBuiltInName`](../setlocalbuiltinname/) снова для той же пары стандартных и локальных имен. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetStandardBuiltInNameWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Создайте пользовательские настройки глобализации
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Установите параметры глобализации для рабочей книги
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Вызовите SetStandardBuiltInName, чтобы сопоставить локальное имя со стандартным встроенным именем
                // Параметры: localName, standardName, bidirectional
                settings.SetStandardBuiltInName("MyLocalName", "SUM", true);
                
                Console.WriteLine("SetStandardBuiltInName executed successfully with parameters (\"MyLocalName\", \"SUM\", true)");
                
                // Продемонстрируйте эффект, используя локальное имя в формуле
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(20);
                worksheet.Cells["A3"].Formula = "=MyLocalName(A1:A2)";
                
                // Вычислите формулу, чтобы показать, что она работает с локальным именем
                workbook.CalculateFormula();
                Console.WriteLine("Result of formula with local name: " + worksheet.Cells["A3"].Value);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetStandardBuiltInName method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("SetStandardBuiltInNameDemo.xlsx");
        }
    }
}
```

### См. также

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


