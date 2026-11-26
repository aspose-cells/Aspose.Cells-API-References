---
title: "SignatureLine.ProviderId"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SignatureLine. Получает или задает идентификатор поставщика подписи"
type: docs
url: /ru/net/aspose.cells.drawing/signatureline/providerid/
---
## SignatureLine.ProviderId property

Получает или задает идентификатор поставщика подписи.

```csharp
public Guid ProviderId { get; set; }
```

### Примечания

Обычно это CLSID COM‑надстройки поставщика.

### Примеры

```csharp
using System;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyProviderIdDemo
    {
        public static void Run()
        {
            // Создать новую строку подписи
            SignatureLine signatureLine = new SignatureLine();
            
            // Установить свойства строки подписи
            signatureLine.Signer = "John Doe";
            signatureLine.Title = "Software Developer";
            signatureLine.Email = "john.doe@example.com";
            signatureLine.IsLine = true;
            
            // Установить идентификатор поставщика (пример GUID — должен быть заменён реальным GUID поставщика)
            signatureLine.ProviderId = new Guid("000CD6A4-0000-0000-C000-000000000046");
            
            // Установить тип подписи (это должно соответствовать идентификатору поставщика)
            signatureLine.SignatureLineType = SignatureType.Stamp;
            
            // Вывести идентификатор поставщика, чтобы продемонстрировать использование
            Console.WriteLine("Signature Line Provider ID: " + signatureLine.ProviderId);
        }
    }
}
```

### См. также

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


