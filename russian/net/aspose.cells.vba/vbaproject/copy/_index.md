---
title: "VbaProject.Copy"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод VbaProject. Копировать VBA проект из другого файла"
type: docs
url: /ru/net/aspose.cells.vba/vbaproject/copy/
---
## VbaProject.Copy method

Копирует проект VBA из другого файла.

```csharp
public void Copy(VbaProject source)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| источник | VbaProject |  |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaProjectMethodCopyWithVbaProjectDemo
    {
        public static void Run()
        {
            Workbook sourceWorkbook = new Workbook();
            int moduleIndex = sourceWorkbook.VbaProject.Modules.Add(VbaModuleType.Procedural, "SourceModule");
            VbaModule sourceModule = sourceWorkbook.VbaProject.Modules[moduleIndex];
            sourceModule.Codes = "Sub SourceMacro()\nMsgBox \"From source\"\nEnd Sub";

            Workbook destWorkbook = new Workbook();

            try
            {
                VbaProject sourceProject = sourceWorkbook.VbaProject;
                VbaProject destProject = destWorkbook.VbaProject;

                destProject.Copy(sourceProject);

                Console.WriteLine($"Copied VBA project '{sourceProject.Name}' to destination workbook. Modules count: {destProject.Modules.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Copy method: {ex.Message}");
            }

            destWorkbook.Save("VbaProjectCopyDemo.xlsx");
        }
    }
}
```

### См. также

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


