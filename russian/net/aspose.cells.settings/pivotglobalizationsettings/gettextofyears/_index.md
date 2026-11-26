---
title: "PivotGlobalizationSettings.GetTextOfYears"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotGlobalizationSettings. Получает локальный текст для Years"
type: docs
url: /ru/net/aspose.cells.settings/pivotglobalizationsettings/gettextofyears/
---
## PivotGlobalizationSettings.GetTextOfYears method

Получает локальный текст "Years".

```csharp
public virtual string GetTextOfYears()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfYearsDemo
    {
        public static void Run()
        {
            // Создайте пользовательские настройки глобализации
            var customSettings = new CustomPivotGlobalizationSettings();
            
            // Продемонстрировать метод GetTextOfYears
            Console.WriteLine("Custom Text of Years: " + customSettings.GetTextOfYears());
        }
    }

    public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
    {
        public override string GetTextOfYears()
        {
            // Возвратить пользовательский текст для метки "Years"
            return "Custom Years Label";
        }
    }
}
```

### См. также

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


