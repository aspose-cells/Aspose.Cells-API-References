---
title: "Класс SignatureLine"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Drawing.SignatureLine класс. Представляет строку подписи"
type: docs
url: /ru/net/aspose.cells.drawing/signatureline/
---
## SignatureLine class

Представляет строку подписи.

```csharp
public class SignatureLine
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [SignatureLine](signatureline/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [AllowComments](../../aspose.cells.drawing/signatureline/allowcomments/) { get; set; } | Указывает, могут ли быть прикреплены комментарии. |
| [Email](../../aspose.cells.drawing/signatureline/email/) { get; set; } | Получает или задает адрес электронной почты исполнителя. |
| [Id](../../aspose.cells.drawing/signatureline/id/) { get; set; } | Получает или задает идентификатор этой строки подписи. |
| [Instructions](../../aspose.cells.drawing/signatureline/instructions/) { get; set; } | Получает или задает текст, отображаемый пользователю во время подписи. |
| [IsLine](../../aspose.cells.drawing/signatureline/isline/) { get; set; } | Указывает, является ли это строкой подписи. |
| [ProviderId](../../aspose.cells.drawing/signatureline/providerid/) { get; set; } | Получает или задает идентификатор поставщика подписи. |
| [ShowSignedDate](../../aspose.cells.drawing/signatureline/showsigneddate/) { get; set; } | Указывает, показывать ли дату подписи. |
| [SignatureLineType](../../aspose.cells.drawing/signatureline/signaturelinetype/) { get; set; } | Получает или задает тип подписи. Default - Когда значение по умолчанию установлено, соответствующее значение ProviderId фиксируется как {0000000000-0000-0000-0000-0000000000}. Stamp - Когда значение равно Stamp, соответствующее значение ProviderId обычно равно {000CD6A4-0000-0000-C000-000000000046}. Custom - Когда значение равно Custom, соответствующее значение ProviderId обычно должно быть задано пользователем. Его следует получить из документации, поставляемой с провайдером. |
| [Signer](../../aspose.cells.drawing/signatureline/signer/) { get; set; } | Получает или задает подписанта. |
| [Title](../../aspose.cells.drawing/signatureline/title/) { get; set; } | Получает или задает заголовок исполнителя. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class SignatureLineDemo
    {
        public static void SignatureLineExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавление изображения
            int imgIndex = worksheet.Pictures.Add(1, 1, "SignatureLineExample_original.png");
            Picture pic = worksheet.Pictures[imgIndex];

            // Создать объект строки подписи.
            SignatureLine s = new SignatureLine();
            s.Signer = "Simon Zhao";
            s.Title = "Development Lead";
            s.Email = "Simon.Zhao@aspose.com";
            s.Id = Guid.NewGuid();
            s.ProviderId = Guid.NewGuid();
            s.IsLine = true;
            s.AllowComments = true;
            s.ShowSignedDate = true;
            s.Instructions = "Just do it.";

            // Назначьте объект строки подписи свойству Picture.SignatureLine
            pic.SignatureLine = s;

            // Сохранить файл Excel
            workbook.Save("SignatureLineExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


