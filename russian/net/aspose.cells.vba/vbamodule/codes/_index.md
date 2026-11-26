---
title: "VbaModule.Codes"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство VbaModule. Получает и задает коды модуля"
type: docs
url: /ru/net/aspose.cells.vba/vbamodule/codes/
---
## VbaModule.Codes property

Получает и задает коды модуля.

```csharp
public string Codes { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModulePropertyCodesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте VBA‑модуль
            int index = workbook.VbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
            Aspose.Cells.Vba.VbaModule module = workbook.VbaProject.Modules[index];
            
            // Установите начальный код
            module.Codes = "Sub TestMacro()\n    MsgBox \"Hello World\"\nEnd Sub";
            
            // Измените код, добавив новые строки
            module.Codes = module.Codes + "\nSub AnotherMacro()\n    MsgBox \"Second Macro\"\nEnd Sub";
            
            // Сохраните книгу
            workbook.Save("VbaModuleDemo.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### См. также

* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


