---
title: "OleObject.AutoUpdate"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство OleObject. Указывает, обновляется ли ссылка на OleObject автоматически или нет."
type: docs
url: /ru/net/aspose.cells.drawing/oleobject/autoupdate/
---
## OleObject.AutoUpdate property

Указывает, обновляется ли ссылка на OleObject автоматически или нет.

```csharp
public bool AutoUpdate { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyAutoUpdateDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Создать образцы файлов для демонстрации
            string imagePath = "OleObjectExample.jpg";
            string excelPath = "OleObjectExample.xls";
            
            // Создать образец изображения, если он не существует
            if (!File.Exists(imagePath))
            {
                using (File.Create(imagePath)) { }
            }

            // Создать образец Excel-файла, если он не существует
            if (!File.Exists(excelPath))
            {
                new Workbook().Save(excelPath);
            }

            // Прочитать данные изображения
            byte[] imageData = File.ReadAllBytes(imagePath);
            
            // Добавить OleObject в лист
            int oleIndex = sheet.OleObjects.Add(1, 1, 200, 200, imageData);
            Aspose.Cells.Drawing.OleObject oleObject = sheet.OleObjects[oleIndex];
            
            // Установить свойства OleObject
            oleObject.ObjectData = File.ReadAllBytes(excelPath);
            oleObject.ProgID = "Excel.Sheet.8";
            oleObject.DisplayAsIcon = true;
            
            // Продемонстрировать свойство AutoUpdate
            oleObject.AutoUpdate = false; // When false, the object won't update automatically when source changes
            
            // Сохраните книгу
            workbook.Save("OleObjectAutoUpdateDemo.xlsx");
        }
    }
}
```

### См. также

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


