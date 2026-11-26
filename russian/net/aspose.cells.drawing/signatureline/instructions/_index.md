---
title: "SignatureLine.Instructions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SignatureLine. Получает или задает текст, отображаемый пользователю во время подписи"
type: docs
url: /ru/net/aspose.cells.drawing/signatureline/instructions/
---
## SignatureLine.Instructions property

Получает или задает текст, отображаемый пользователю во время подписи.

```csharp
public string Instructions { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyInstructionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать объект строки подписи
            SignatureLine signatureLine = new SignatureLine();
            signatureLine.Instructions = "Please sign here after reviewing the document.";

            // Добавить строку подписи в лист в позицию (1,1)
            worksheet.Shapes.AddSignatureLine(1, 1, signatureLine);

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


