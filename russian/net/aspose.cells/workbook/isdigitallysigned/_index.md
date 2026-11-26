---
title: "Workbook.IsDigitallySigned"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Workbook. Указывает, подписана ли эта электронная таблица цифровой подписью"
type: docs
url: /ru/net/aspose.cells/workbook/isdigitallysigned/
---
## Workbook.IsDigitallySigned property

Указывает, подписана ли эта электронная таблица цифровой подписью.

```csharp
public bool IsDigitallySigned { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyIsDigitallySignedDemo
    {
        public static void Run()
        {
            // Загрузить цифрово подписанную книгу Workbook
            Workbook book = new Workbook("Test_DigiSign.xlsx");
            
            // Проверить, подписана ли книга цифровой подписью
            bool isSigned = book.IsDigitallySigned;
            Console.WriteLine("Workbook is digitally signed: " + isSigned);

            if (isSigned)
            {
                // Сохранить копию (подпись будет сохранена)
                book.Save("SignedCopy.xlsx");
                
                // Удалить цифровую подпись
                book.RemoveDigitalSignature();
                book.Save("UnsignedCopy.xlsx");
                
                // Проверить, что подпись удалена
                Workbook unsignedBook = new Workbook("UnsignedCopy.xlsx");
                Console.WriteLine("After removal, workbook is signed: " + unsignedBook.IsDigitallySigned);
            }
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


