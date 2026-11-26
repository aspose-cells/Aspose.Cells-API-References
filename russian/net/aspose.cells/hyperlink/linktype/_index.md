---
title: "Hyperlink.LinkType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Hyperlink. Получает тип ссылки"
type: docs
url: /ru/net/aspose.cells/hyperlink/linktype/
---
## Hyperlink.LinkType property

Получает тип ссылки.

```csharp
public TargetModeType LinkType { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkPropertyLinkTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить внешнюю гиперссылку
            int hyperlinkIndex = worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            Hyperlink link = worksheet.Hyperlinks[hyperlinkIndex];
            
            // Продемонстрировать свойство LinkType
            Console.WriteLine("Hyperlink LinkType: " + link.LinkType);
            
            // Очистить
            link.Delete();
            Console.WriteLine("Hyperlinks count after deletion: " + worksheet.Hyperlinks.Count);
        }
    }
}
```

### См. также

* enum [TargetModeType](../../targetmodetype/)
* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


