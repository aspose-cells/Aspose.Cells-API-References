---
title: "CellsHelper.IsCloudPlatform"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CellsHelper. Пожалуйста, установите это свойство в True при работе на облачной платформе, такой как Azure, AWSLambda и т.д."
type: docs
url: /ru/net/aspose.cells/cellshelper/iscloudplatform/
---
## CellsHelper.IsCloudPlatform property

Пожалуйста, установите это свойство в значение True при работе на облачной платформе, такой как: Azure, AWSLambda и т.д.

```csharp
public static bool IsCloudPlatform { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyIsCloudPlatformDemo
    {
        public static void Run()
        {
            // Задать свойство IsCloudPlatform
            CellsHelper.IsCloudPlatform = true;

            // Продемонстрировать использование свойства
            Console.WriteLine("Is Cloud Platform: " + CellsHelper.IsCloudPlatform);

            // Показать, как это влияет на другие операции (пример)
            if (CellsHelper.IsCloudPlatform)
            {
                Console.WriteLine("Running in cloud environment - using cloud-specific settings");
                CellsHelper.StartupPath = "/cloud_storage/aspose/cells";
            }
            else
            {
                Console.WriteLine("Running in local environment");
                CellsHelper.StartupPath = "C:\\Program Files\\Aspose\\Cells";
            }
        }
    }
}
```

### См. также

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


