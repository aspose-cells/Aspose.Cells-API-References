---
title: "DocumentPropertyCollection.Remove"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод DocumentPropertyCollection. Удаляет свойство с указанным именем из коллекции"
type: docs
url: /ru/net/aspose.cells.properties/documentpropertycollection/remove/
---
## DocumentPropertyCollection.Remove method

Удаляет свойство с указанным именем из коллекции.

```csharp
public void Remove(string name)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя свойства без учёта регистра. |

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocumentPropertyCollectionMethodRemoveWithStringDemo
    {
        public static void Run()
        {
            string inputPath = "example.xlsx";
            string outputPath = "output.xlsm";

            using (FileStream stream = new FileStream(inputPath, FileMode.Open))
            {
                Workbook workbook = new Workbook(stream);
                
                if (workbook.Worksheets.CustomDocumentProperties.Contains("_PID_HLINKS"))
                {
                    workbook.Worksheets.CustomDocumentProperties.Remove("_PID_HLINKS");
                }

                workbook.Save(outputPath, SaveFormat.Xlsm);
            }
        }
    }
}
```

### См. также

* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


