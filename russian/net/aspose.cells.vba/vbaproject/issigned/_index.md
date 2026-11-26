---
title: "VbaProject.IsSigned"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство VbaProject. Указывает, подписан ли VBAcode или нет"
type: docs
url: /ru/net/aspose.cells.vba/vbaproject/issigned/
---
## VbaProject.IsSigned property

Указывает, подписан ли VBAcode или нет.

```csharp
public bool IsSigned { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyIsSignedDemo
    {
        public static void Run()
        {
            // Загрузить пример файла Excel с VBA проектом
            Workbook workbook = new Workbook("example.xlsm");
            
            // Проверьте, подписан ли VBA проект
            if (workbook.VbaProject.IsSigned)
            {
                Console.WriteLine("VBA project is signed.");
                Console.WriteLine("Signature is valid: " + workbook.VbaProject.IsValidSigned);
            }
            else
            {
                Console.WriteLine("VBA project is not signed.");
            }
        }
    }
}
```

### См. также

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


