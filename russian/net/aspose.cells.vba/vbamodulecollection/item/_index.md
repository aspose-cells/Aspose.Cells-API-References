---
title: "VbaModuleCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство VbaModuleCollection. Получает VbaModule в списке по индексу"
type: docs
url: /ru/net/aspose.cells.vba/vbamodulecollection/item/
---
## VbaModuleCollection indexer (1 of 2)

Получает [`VbaModule`](../../vbamodule/) в списке по индексу.

```csharp
public VbaModule this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Создайте новую книгу с проектом VBA
            Workbook workbook = new Workbook("sample.xlsm");
            
            // Получите существующий проект VBA (VbaProject только для чтения)
            VbaProject vbaProject = workbook.VbaProject;
            
            // Добавьте модуль в проект VBA
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
            
            // Получите доступ к модулю, используя свойство Item
            VbaModule module = vbaProject.Modules[index];
            
            // Добавьте некоторый код VBA в модуль
            module.Codes = "Sub TestMacro()\n    MsgBox \"Hello from VBA!\"\nEnd Sub";
            
            // Сохраните книгу
            workbook.Save("VbaModuleDemo.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### См. также

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)

---

## VbaModuleCollection indexer (2 of 2)

Получает [`VbaModule`](../../vbamodule/) в списке по имени.

```csharp
public VbaModule this[string name] { get; }
```

| Параметр | Описание |
| --- | --- |
| name | Имя модуля. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить лист
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте модуль VBA в книгу
            int moduleIndex = workbook.VbaProject.Modules.Add(worksheet);
            
            // Получите доступ к модулю, используя свойство Item по имени
            VbaModule module = workbook.VbaProject.Modules[worksheet.CodeName];
            
            // Установите код VBA
            module.Codes = "Sub Test()\r\n    MsgBox \"Hello World!\"\r\nEnd Sub";
            
            // Сохраните книгу
            workbook.Save("output.xlsm", SaveFormat.Xlsm);
            
            // Проверить, загрузив обратно
            Workbook verifyWorkbook = new Workbook("output.xlsm");
            VbaModule verifyModule = verifyWorkbook.VbaProject.Modules[worksheet.CodeName];
            
            Console.WriteLine("VBA Code in saved file:");
            Console.WriteLine(verifyModule.Codes);
        }
    }
}
```

### См. также

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


