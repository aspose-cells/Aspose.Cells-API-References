---
title: "SignatureLine.Id"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SignatureLine. Получает или задает идентификатор этой строки подписи"
type: docs
url: /ru/net/aspose.cells.drawing/signatureline/id/
---
## SignatureLine.Id property

Получает или задает идентификатор этой строки подписи.

```csharp
public Guid Id { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyIdDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать объект строки подписи
            SignatureLine signatureLine = new SignatureLine();
            Guid signatureId = Guid.NewGuid();
            signatureLine.Id = signatureId;
            
            // Добавить строку подписи в лист в позицию (1,1)
            worksheet.Shapes.AddSignatureLine(0, 0, signatureLine);

            // Отобразить идентификатор строки подписи
            Console.WriteLine("Signature Line ID: " + signatureLine.Id);
        }
    }
}
```

### См. также

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


