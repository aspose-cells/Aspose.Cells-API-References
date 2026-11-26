---
title: "ReferredArea.ExternalFileName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ReferredArea. Получить имя внешнего файла, если это внешняя ссылка"
type: docs
url: /ru/net/aspose.cells/referredarea/externalfilename/
---
## ReferredArea.ExternalFileName property

Получить имя внешнего файла, если это внешняя ссылка.

```csharp
public string ExternalFileName { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaPropertyExternalFileNameDemo
    {
        public static void Run()
        {
            // Создать книгу с внешней ссылкой
            Workbook wb = new Workbook();
            
            // Создать имя, которое ссылается на внешнюю книгу
            int index = wb.Worksheets.Names.Add("RefExternalName");
            wb.Worksheets.Names[index].RefersTo = "='[ExternalLinkSource.xlsx]Sheet1'!$A$1:$C$3";
            
            // Получить ссылочную область
            ReferredArea ra = wb.Worksheets.Names["RefExternalName"].GetReferredAreas(false)[0];
            
            // Продемонстрировать свойство ExternalFileName
            Console.WriteLine("External File Name: " + ra.ExternalFileName);
            Console.WriteLine("Sheet Name: " + ra.SheetName);
            Console.WriteLine("Area: R" + ra.StartRow + "C" + ra.StartColumn + 
                              " to R" + ra.EndRow + "C" + ra.EndColumn);
            
            // Проверить имя внешнего файла
            if (!ra.ExternalFileName.EndsWith("ExternalLinkSource.xlsx"))
            {
                Console.WriteLine("Error: ExternalFileName should be ExternalLinkSource.xlsx");
            }
        }
    }
}
```

### См. также

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


