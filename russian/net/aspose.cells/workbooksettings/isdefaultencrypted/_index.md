---
title: "WorkbookSettings.IsDefaultEncrypted"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Указывает, будет ли книга зашифрована паролем по умолчанию, если структура и окна книги заблокированы"
type: docs
url: /ru/net/aspose.cells/workbooksettings/isdefaultencrypted/
---
## WorkbookSettings.IsDefaultEncrypted property

Указывает, шифровать ли рабочую книгу паролем по умолчанию, если структура и окна рабочей книги заблокированы.

```csharp
public bool IsDefaultEncrypted { get; set; }
```

### Примечания

Значение по умолчанию сейчас — false. Это то же самое, что в MS Excel 2013.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsDefaultEncryptedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook(FileFormatType.Xlsx);
            Console.WriteLine("IsDefaultEncrypted: " + workbook.Settings.IsDefaultEncrypted);
            
            workbook.Settings.IsDefaultEncrypted = true;
            Console.WriteLine("After setting to true: " + workbook.Settings.IsDefaultEncrypted);
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


