---
title: "SignatureLine.Email"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SignatureLine. Получает или задает электронную почту подписанта"
type: docs
url: /ru/net/aspose.cells.drawing/signatureline/email/
---
## SignatureLine.Email property

Получает или задает адрес электронной почты исполнителя.

```csharp
public string Email { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyEmailDemo
    {
        public static void Run()
        {
            // Создать новую строку подписи
            SignatureLine signatureLine = new SignatureLine();
            
            // Установить свойства строки подписи, включая Email
            signatureLine.Signer = "Simon Zhao";
            signatureLine.Title = "Software Developer";
            signatureLine.Email = "Simon.Zhao@aspose.com";
            signatureLine.IsLine = true;
            signatureLine.ShowSignedDate = true;
            
            // Отобразить свойство email
            Console.WriteLine("Signer Email: " + signatureLine.Email);
        }
    }
}
```

### См. также

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


