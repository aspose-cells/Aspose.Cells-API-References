---
title: "OleObject.DisplayAsIcon"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство OleObject. Истина, если указанный объект отображается как значок, и изображение не будет автоматически изменено"
type: docs
url: /ru/net/aspose.cells.drawing/oleobject/displayasicon/
---
## OleObject.DisplayAsIcon property

True, если указанный объект отображается как значок и изображение не будет автоматически изменено.

```csharp
public bool DisplayAsIcon { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyDisplayAsIconDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте OLE‑объект (PDF) в лист
            byte[] pdfData = File.ReadAllBytes("example.pdf");
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, pdfData);
            
            // Получите OLE‑объект
            Aspose.Cells.Drawing.OleObject oleObject = worksheet.OleObjects[oleIndex];
            oleObject.ProgID = "AcroExch.Document.DC";
            
            // Продемонстрируйте свойство DisplayAsIcon
            oleObject.DisplayAsIcon = true; // Show as icon
            // oleObject.DisplayAsIcon = false; // Показать содержимое, если возможно
            
            // Сохраните книгу
            workbook.Save("OleObjectDisplayAsIconDemo.xlsx");
        }
    }
}
```

### См. также

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


