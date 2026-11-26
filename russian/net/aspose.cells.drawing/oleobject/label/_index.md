---
title: "OleObject.Label"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство OleObject. Получает и задаёт отображаемый ярлык связанного ole‑объекта"
type: docs
url: /ru/net/aspose.cells.drawing/oleobject/label/
---
## OleObject.Label property

Получает и задает отображаемую метку связанного ole‑объекта.

```csharp
public string Label { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyLabelDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте OLE‑объект с ярлыком
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0]);
            OleObject oleObject = worksheet.OleObjects[oleIndex];
            oleObject.Label = "label_nameです";

            // Сохранить и перезагрузить книгу
            string outputPath = "output.xlsx";
            workbook.Save(outputPath);
            
            // Проверьте свойство label
            Workbook loadedWorkbook = new Workbook(outputPath);
            OleObject loadedOleObject = loadedWorkbook.Worksheets[0].OleObjects[0];
            Console.WriteLine("OLE Object Label: " + loadedOleObject.Label);
        }
    }
}
```

### См. также

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


