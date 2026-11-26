---
title: "CopyOptions.KeepMacros"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CopyOptions. Указывает, сохраняются ли макросы"
type: docs
url: /ru/net/aspose.cells/copyoptions/keepmacros/
---
## CopyOptions.KeepMacros property

Указывает, сохранять ли макросы;

```csharp
public bool KeepMacros { get; set; }
```

### Примечания

Только для копирования рабочей книги.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyKeepMacrosDemo
    {
        public static void Run()
        {
            // Создайте исходную рабочую книгу с макросами (используя файл шаблона, содержащий макросы)
            Workbook srcWorkbook = new Workbook("macros_template.xlsm");
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            srcSheet.Cells["A1"].PutValue("Macro-enabled source");

            // Создайте целевую книгу
            Workbook destWorkbook = new Workbook();
            
            // Установите параметры копирования с KeepMacros true
            CopyOptions options = new CopyOptions();
            options.KeepMacros = true;

            // Скопировать лист с макросами
            destWorkbook.Worksheets[0].Copy(srcSheet, options);

            // Сохранить результат
            destWorkbook.Save("KeepMacrosExample.xlsm");
        }
    }
}
```

### См. также

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


