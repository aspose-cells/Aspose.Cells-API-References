---
title: "SignatureLine.Signer"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SignatureLine. Получает или задает подписанта"
type: docs
url: /ru/net/aspose.cells.drawing/signatureline/signer/
---
## SignatureLine.Signer property

Получает или задает подписанта.

```csharp
public string Signer { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertySignerDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать строку подписи и установить её свойства
            SignatureLine signatureLine = new SignatureLine();
            signatureLine.Signer = "John Doe";
            signatureLine.Title = "Software Developer";
            signatureLine.Email = "john.doe@example.com";

            // Добавить строку подписи в лист в ячейку строки 1, столбца 1
            worksheet.Shapes.AddSignatureLine(0, 0, signatureLine);

            // Сохраните книгу
            workbook.Save("SignatureLineDemo.xlsx");
        }
    }
}
```

### См. также

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


