---
title: "VbaModuleCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод VbaModuleCollection. Добавляет модуль для рабочего листа"
type: docs
url: /ru/net/aspose.cells.vba/vbamodulecollection/add/
---
## Add(Worksheet) {#add_1}

Добавляет модуль для листа.

```csharp
public int Add(Worksheet sheet)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| лист | Worksheet | Рабочий лист |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionMethodAddWithWorksheetDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте модуль VBA, связанный с рабочим листом
            int moduleIndex = workbook.VbaProject.Modules.Add(worksheet);
            
            // Добавьте некоторый код VBA в модуль
            string vbaCode = "Sub Test()\n    MsgBox \"Hello from VBA!\"\nEnd Sub";
            workbook.VbaProject.Modules[moduleIndex].Codes = vbaCode;
            
            // Сохраните книгу с проектом VBA
            workbook.Save("output.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### См. также

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)

---

## Add(VbaModuleType, string) {#add}

Добавляет модуль.

```csharp
public int Add(VbaModuleType type, string name)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| type | VbaModuleType | Тип модуля. |
| name | String | Имя модуля. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionMethodAddWithVbaModuleTypeStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            VbaProject vbaProject = workbook.VbaProject;

            int index = vbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
            VbaModule module = vbaProject.Modules[index];
            module.Codes = "Sub Test()\r\nMsgBox \"Hello World\"\r\nEnd Sub";

            workbook.Save("VbaModuleAddExample.xlsm");
        }
    }
}
```

### См. также

* enum [VbaModuleType](../../vbamoduletype/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


