---
title: "SignatureLine.SignatureLineType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SignatureLine. Получает или задает тип подписи. Default  Когда значение Default установлено, соответствующее значение ProviderId фиксируется как 00000000000000000000000000000000. Stamp  Когда значение равно Stamp, соответствующее значение ProviderId обычно равно 000CD6A400000000C000000000000046. Custom  Когда значение равно Custom, соответствующее значение ProviderId обычно должно быть задано пользователем. его следует получить из документации, поставляемой с провайдером"
type: docs
url: /ru/net/aspose.cells.drawing/signatureline/signaturelinetype/
---
## SignatureLine.SignatureLineType property

Получает или задает тип подписи. Default - Когда значение по умолчанию установлено, соответствующее значение ProviderId фиксируется как {0000000000-0000-0000-0000-0000000000}. Stamp - Когда значение равно Stamp, соответствующее значение ProviderId обычно равно {000CD6A4-0000-0000-C000-000000000046}. Custom - Когда значение равно Custom, соответствующее значение ProviderId обычно должно быть задано пользователем. Его следует получить из документации, поставляемой с провайдером.

```csharp
public SignatureType SignatureLineType { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class SignatureLinePropertySignatureLineTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать строку подписи
            SignatureLine signatureLine = new SignatureLine();
            signatureLine.Signer = "John Doe";
            signatureLine.Title = "Developer";
            signatureLine.Email = "john@example.com";
            signatureLine.IsLine = true;
            signatureLine.AllowComments = true;
            signatureLine.ShowSignedDate = true;
            signatureLine.Instructions = "Please sign here";

            // Отобразить текущий SignatureLineType
            Console.WriteLine("Current SignatureLineType: " + signatureLine.SignatureLineType);

            // Установить SignatureLineType в Stamp
            signatureLine.SignatureLineType = SignatureType.Stamp;
            Console.WriteLine("Changed SignatureLineType to: " + signatureLine.SignatureLineType);
            Console.WriteLine("ProviderId after Stamp type: " + signatureLine.ProviderId);

            // Добавить строку подписи в лист, добавив её в фигуры
            Picture signaturePicture = worksheet.Shapes.AddSignatureLine(0, 0, signatureLine); // Changed to Picture type
            Console.WriteLine("Added signature line with index: " + signaturePicture.OriginalHeight);

            // Изменить SignatureLineType на Custom с пользовательским ProviderId
            signatureLine.SignatureLineType = SignatureType.Custom;
            signatureLine.ProviderId = Guid.NewGuid();
            Console.WriteLine("Changed SignatureLineType to: " + signatureLine.SignatureLineType);
            Console.WriteLine("Custom ProviderId: " + signatureLine.ProviderId);

            // Сохраните книгу
            workbook.Save("SignatureLineTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [SignatureType](../../signaturetype/)
* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


