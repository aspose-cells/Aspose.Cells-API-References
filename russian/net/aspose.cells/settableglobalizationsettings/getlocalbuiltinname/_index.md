---
title: "SettableGlobalizationSettings.GetLocalBuiltInName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableGlobalizationSettings. Получает зависящий от локали текст для встроенного Name в соответствии с заданным стандартным текстом"
type: docs
url: /ru/net/aspose.cells/settableglobalizationsettings/getlocalbuiltinname/
---
## SettableGlobalizationSettings.GetLocalBuiltInName method

Получает текст встроенного имени, зависящий от локали, в соответствии с заданным стандартным текстом.

```csharp
public override string GetLocalBuiltInName(string standardName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| standardName | String | Текст стандартного (en-US) встроенного Name. |

### Возвращаемое значение

Текст, зависящий от локали. Локаль была указана Workbook, для которого используются эти настройки.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetLocalBuiltInNameWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте экземпляр SettableGlobalizationSettings
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

            try
            {
                // Вызвать метод GetLocalBuiltInName со стандартным встроенным именем
                string standardName = "SUM";
                string localName = globalizationSettings.GetLocalBuiltInName(standardName);

                // Отобразить результат
                Console.WriteLine($"Standard name: {standardName}, Local name: {localName}");

                // Установить пользовательское локальное имя для стандартного встроенного имени
                globalizationSettings.SetLocalBuiltInName(standardName, "CustomSum", true);

                // Получить локальное имя снова после его установки
                localName = globalizationSettings.GetLocalBuiltInName(standardName);
                Console.WriteLine($"After setting - Standard name: {standardName}, Local name: {localName}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetLocalBuiltInName method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("MethodGetLocalBuiltInNameDemo.xlsx");
        }
    }
}
```

### См. также

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


