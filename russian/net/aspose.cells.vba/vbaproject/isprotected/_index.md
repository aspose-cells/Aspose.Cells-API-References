---
title: "VbaProject.IsProtected"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство VbaProject. Указывает, защищён ли данный VBA проект"
type: docs
url: /ru/net/aspose.cells.vba/vbaproject/isprotected/
---
## VbaProject.IsProtected property

Указывает, защищён ли этот VBA‑проект.

```csharp
public bool IsProtected { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyIsProtectedDemo
    {
        public static void Run()
        {
            // Загрузить пример файла Excel с незащищённым VBA проектом
            Workbook wb = new Workbook("load.xlsm");
            VbaProject vbaProject = wb.VbaProject;
            Console.WriteLine("Is VBA Project Protected (load.xlsm): " + vbaProject.IsProtected);
            Console.WriteLine("Is VBA Project Locked for Viewing: " + vbaProject.IslockedForViewing);

            // Загрузить пример файла Excel с защищённым VBA проектом
            wb = new Workbook("load_protected.xlsm");
            vbaProject = wb.VbaProject;
            Console.WriteLine("Is VBA Project Protected (load_protected.xlsm): " + vbaProject.IsProtected);
            Console.WriteLine("Is VBA Project Locked for Viewing: " + vbaProject.IslockedForViewing);

            // Загрузить пример файла Excel с защищённым и заблокированным VBA проектом
            wb = new Workbook("load_protected_lockedForView.xlsm");
            vbaProject = wb.VbaProject;
            Console.WriteLine("Is VBA Project Protected (load_protected_lockedForView.xlsm): " + vbaProject.IsProtected);
            Console.WriteLine("Is VBA Project Locked for Viewing: " + vbaProject.IslockedForViewing);
        }
    }
}
```

### См. также

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


