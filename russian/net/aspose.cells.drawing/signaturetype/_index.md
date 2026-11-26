---
title: "Перечисление SignatureType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.SignatureType. Указывает тип подписи"
type: docs
url: /ru/net/aspose.cells.drawing/signaturetype/
---
## SignatureType enumeration

Указывает тип подписи.

```csharp
public enum SignatureType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Default | `0` | Значение по умолчанию, соответствующее значение ProviderId фиксировано как {0000000000-0000-0000-0000-0000000000}. |
| Stamp | `1` | Соответствующее значение ProviderId обычно равно {000CD6A4-0000-0000-C000-000000000046}. |
| Custom | `3` | Обычно соответствующее значение ProviderId должно устанавливаться пользователем. Оно должно быть получено из документации, поставляемой с провайдером. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassSignatureTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить строки подписи с разными типами
            Picture stampPicture = worksheet.Shapes.AddSignatureLine(3, 1, new SignatureLine());
            stampPicture.SignatureLine.SignatureLineType = SignatureType.Stamp;

            Picture customPicture = worksheet.Shapes.AddSignatureLine(8, 1, new SignatureLine());
            customPicture.SignatureLine.SignatureLineType = SignatureType.Custom;
            customPicture.SignatureLine.ProviderId = new Guid("12345678-ABCD-4321-5678-9876543210AB");

            // Сохранить книгу с настройками подписи
            workbook.Save("SignatureTypeDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


