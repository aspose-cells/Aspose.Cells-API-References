---
title: "Workbook.VbaProject"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Workbook. Получает VbaProject в электронной таблице"
type: docs
url: /ru/net/aspose.cells/workbook/vbaproject/
---
## Workbook.VbaProject property

Получает `VbaProject` в электронной таблице.

```csharp
public VbaProject VbaProject { get; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyVbaProjectDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Доступ к проекту VBA (VbaProject доступен только для чтения, мы можем лишь проверить его наличие)
            if (workbook.VbaProject == null)
            {
                // Создать проект VBA, сохранив как книгу с поддержкой макросов
                workbook.Save("temp.xlsm", SaveFormat.Xlsm);
                workbook = new Workbook("temp.xlsm");
                File.Delete("temp.xlsm");
            }

            // Добавить новый модуль в проект VBA
            int moduleIndex = workbook.VbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
            
            // Получить добавленный модуль и задать его код
            VbaModule module = workbook.VbaProject.Modules[moduleIndex];
            module.Codes = "Sub Test()\r\n    MsgBox \"Hello from VBA!\"\r\nEnd Sub";

            // Сохраните книгу
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "VbaProjectDemo.xlsm");
            workbook.Save(outputPath, SaveFormat.Xlsm);
        }
    }
}
```

### См. также

* class [VbaProject](../../../aspose.cells.vba/vbaproject/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


