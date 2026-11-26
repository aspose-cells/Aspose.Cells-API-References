---
title: "SignatureLine.Title"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SignatureLine. Получает или задает заголовок подписанта"
type: docs
url: /ru/net/aspose.cells.drawing/signatureline/title/
---
## SignatureLine.Title property

Получает или задает заголовок исполнителя.

```csharp
public string Title { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyTitleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать строку подписи и задать её заголовок
            SignatureLine signatureLine = new SignatureLine();
            signatureLine.Title = "Development Lead";

            // Добавить строку подписи в формы листа с параметрами позиции
            worksheet.Shapes.AddSignatureLine(0, 0, signatureLine);

            // Вывести заголовок, чтобы продемонстрировать, что свойство было установлено
            Console.WriteLine("Signature Line Title: " + signatureLine.Title);
        }
    }
}
```

### См. также

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


