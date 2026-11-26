---
title: "SignatureLine.IsLine"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SignatureLine. Указывает, является ли это строкой подписи"
type: docs
url: /ru/net/aspose.cells.drawing/signatureline/isline/
---
## SignatureLine.IsLine property

Указывает, является ли это строкой подписи.

```csharp
public bool IsLine { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyIsLineDemo
    {
        public static void Run()
        {
            // Создать экземпляр строки подписи
            SignatureLine signature = new SignatureLine();
            
            // Установить IsLine в true
            signature.IsLine = true;
            
            // Проверить и продемонстрировать использование IsLine
            if (signature.IsLine)
            {
                Console.WriteLine("Signature line is active.");
            }
            
            // Переключить состояние IsLine
            signature.IsLine = false;
            
            if (!signature.IsLine)
            {
                Console.WriteLine("Signature line is now inactive.");
            }
        }
    }
}
```

### См. также

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


