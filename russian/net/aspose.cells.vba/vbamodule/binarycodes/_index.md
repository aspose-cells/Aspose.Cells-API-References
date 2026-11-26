---
title: "VbaModule.BinaryCodes"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство VbaModule. Получает и задает бинарные коды модуля"
type: docs
url: /ru/net/aspose.cells.vba/vbamodule/binarycodes/
---
## VbaModule.BinaryCodes property

Получает и задает бинарные коды модуля.

```csharp
public byte[] BinaryCodes { get; }
```

### Примеры

```csharp
using System;
using System.Text;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModulePropertyBinaryCodesDemo
    {
        public static void Run()
        {
            // Загрузите рабочую книгу с VBA‑проектом
            Workbook workbook = new Workbook("example.xlsm");
            
            // Доступ к проекту VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // Получите бинарные коды из первого модуля
            byte[] binaryCodes = vbaProject.Modules[0].BinaryCodes;
            
            // Преобразуйте в строку, используя китайскую кодировку (936)
            string codeContent = Encoding.GetEncoding(936).GetString(binaryCodes);
            
            // Выведите содержимое, содержащее китайские символы
            Console.WriteLine("VBA Module Content:");
            Console.WriteLine(codeContent);
        }
    }
}
```

### См. также

* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


