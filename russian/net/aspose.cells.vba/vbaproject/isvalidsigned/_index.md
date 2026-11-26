---
title: "VbaProject.IsValidSigned"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство VbaProject. Указывает, действительна ли подпись проекта VBA или нет"
type: docs
url: /ru/net/aspose.cells.vba/vbaproject/isvalidsigned/
---
## VbaProject.IsValidSigned property

Указывает, действительна ли подпись проекта VBA или нет.

```csharp
public bool IsValidSigned { get; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyIsValidSignedDemo
    {
        public static void Run()
        {
            // Загрузить пример рабочей книги с подписанным проектом VBA
            Workbook wb = new Workbook("example.xlsm");
            
            // Проверить, подписан ли проект VBA и действительна ли подпись
            Console.WriteLine("Is VBA Project Signed: " + wb.VbaProject.IsSigned);
            Console.WriteLine("Is Signature Valid: " + wb.VbaProject.IsValidSigned);

            // Сохранить и перезагрузить, чтобы проверить сохранность подписи
            MemoryStream ms = new MemoryStream();
            wb.Save(ms, SaveFormat.Excel97To2003);
            
            Workbook validateWb = new Workbook(ms);
            Console.WriteLine("After Reload - Is VBA Project Signed: " + validateWb.VbaProject.IsSigned);
            Console.WriteLine("After Reload - Is Signature Valid: " + validateWb.VbaProject.IsValidSigned);
        }
    }
}
```

### См. также

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


