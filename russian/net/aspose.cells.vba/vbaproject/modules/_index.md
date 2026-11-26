---
title: "VbaProject.Modules"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство VbaProject. Получает все объекты VbaModule"
type: docs
url: /ru/net/aspose.cells.vba/vbaproject/modules/
---
## VbaProject.Modules property

Получает все объекты [`VbaModule`](../../vbamodule/).

```csharp
public VbaModuleCollection Modules { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyModulesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            VbaProject vbaProject = workbook.VbaProject;
            
            // Добавьте новый модуль и получите его с помощью свойства Modules
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
            VbaModule module = vbaProject.Modules[index];
            
            // Добавьте код в модуль
            module.Codes = "Sub Test()\r\n    MsgBox \"Module demonstration\"\r\nEnd Sub";
            
            // Сохранить в формате с поддержкой макросов
            workbook.Save("VbaModulesDemo.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### См. также

* class [VbaModuleCollection](../../vbamodulecollection/)
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


