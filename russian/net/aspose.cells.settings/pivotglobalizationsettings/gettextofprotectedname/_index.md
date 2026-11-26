---
title: "PivotGlobalizationSettings.GetTextOfProtectedName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotGlobalizationSettings. Получает текст для указанного защищённого имени"
type: docs
url: /ru/net/aspose.cells.settings/pivotglobalizationsettings/gettextofprotectedname/
---
## PivotGlobalizationSettings.GetTextOfProtectedName method

Получает текст для указанного защищённого имени.

```csharp
public virtual string GetTextOfProtectedName(string protectedName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| protectedName | String | Защищённое имя в сводной таблице. |

### Возвращаемое значение

Локальные защищённые имена сводной таблицы.

### Примечания

В Microsoft Excel некоторые имена нельзя использовать в качестве названий полей PivotFields в сводной таблице. Они различаются в разных регионах, пользователь может явно указать их в соответствии с используемым регионом.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfProtectedNameWithStringDemo
    {
        public static void Run()
        {
            try
            {
                // Создайте экземпляр PivotGlobalizationSettings
                PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

                // Определите защищённое имя, чтобы получить его текст
                string protectedName = "SensitiveData";

                // Вызовите метод GetTextOfProtectedName
                string result = globalizationSettings.GetTextOfProtectedName(protectedName);

                // Вывести результат.
                Console.WriteLine($"Text for protected name \"{protectedName}\": {result}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfProtectedName: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


