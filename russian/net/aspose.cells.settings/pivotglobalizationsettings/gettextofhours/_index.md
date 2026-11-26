---
title: "PivotGlobalizationSettings.GetTextOfHours"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotGlobalizationSettings. Получает локальный текст часов"
type: docs
url: /ru/net/aspose.cells.settings/pivotglobalizationsettings/gettextofhours/
---
## PivotGlobalizationSettings.GetTextOfHours method

Получает локальный текст "Hours".

```csharp
public virtual string GetTextOfHours()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfHoursDemo
    {
        public static void Run()
        {
            // Создайте экземпляр PivotGlobalizationSettings
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

            // Продемонстрируйте метод GetTextOfHours
            Console.WriteLine("Text of Hours: " + globalizationSettings.GetTextOfHours());

            // Дополнительная демонстрация связанных методов времени
            Console.WriteLine("Text of Minutes: " + globalizationSettings.GetTextOfMinutes());
            Console.WriteLine("Text of Seconds: " + globalizationSettings.GetTextOfSeconds());
        }
    }
}
```

### См. также

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


