---
title: "PivotGlobalizationSettings.GetTextOfMinutes"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotGlobalizationSettings. Получает локальный текст минут"
type: docs
url: /ru/net/aspose.cells.settings/pivotglobalizationsettings/gettextofminutes/
---
## PivotGlobalizationSettings.GetTextOfMinutes method

Получает локальный текст "Minutes".

```csharp
public virtual string GetTextOfMinutes()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfMinutesDemo
    {
        public static void Run()
        {
            // Создайте экземпляр PivotGlobalizationSettings
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

            // Продемонстрировать метод GetTextOfMinutes
            Console.WriteLine("Text of Minutes: " + globalizationSettings.GetTextOfMinutes());

            // Дополнительная демонстрация связанных методов времени для контекста
            Console.WriteLine("Text of Hours: " + globalizationSettings.GetTextOfHours());
            Console.WriteLine("Text of Seconds: " + globalizationSettings.GetTextOfSeconds());
        }
    }
}
```

### См. также

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


