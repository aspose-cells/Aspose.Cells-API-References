---
title: "VbaProject.Encoding"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство VbaProject. Получает и задает кодировку проекта VBA"
type: docs
url: /ru/net/aspose.cells.vba/vbaproject/encoding/
---
## VbaProject.Encoding property

Получает и задаёт кодировку VBA‑проекта.

```csharp
public Encoding Encoding { get; set; }
```

### Примеры

```csharp
using System;
using System.Text;
using Aspose.Cells;
using Aspose.Cells.Vba;
using System.Security.Cryptography.X509Certificates;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyEncodingDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Инициализировать проект VBA
            VbaProject vbaProject = workbook.VbaProject;

            // Установить свойства проекта VBA, включая кодировку
            vbaProject.Name = "TestVbaProject";
            vbaProject.Encoding = Encoding.UTF8;

            // Добавьте модуль в проект VBA
            vbaProject.Modules.Add(VbaModuleType.Class, "TestModule");

            // Сохраните книгу с проектом VBA
            workbook.Save("VbaProjectEncodingDemo.xlsm");
        }
    }
}
```

### См. также

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


