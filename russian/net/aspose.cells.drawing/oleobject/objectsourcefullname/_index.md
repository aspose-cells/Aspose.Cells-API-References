---
title: "OleObject.ObjectSourceFullName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство OleObject. Возвращает полное имя исходного файла для связанного OLE‑объекта"
type: docs
url: /ru/net/aspose.cells.drawing/oleobject/objectsourcefullname/
---
## OleObject.ObjectSourceFullName property

Возвращает полное имя исходного файла для связанного OLE‑объекта.

```csharp
public string ObjectSourceFullName { get; set; }
```

### Примечания

Поддерживает установку полного имени источника только когда тип файла OleFileType.Unknown. Например, файлы wav, avi и т.д.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyObjectSourceFullNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить OLE‑объект (используя данные файла в виде массива байтов)
            byte[] fileData = System.IO.File.ReadAllBytes("test.docx");
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, fileData);
            Aspose.Cells.Drawing.OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            // Установить и получить ObjectSourceFullName
            oleObject.ObjectSourceFullName = "C:\\Temp\\source.docx";
            Console.WriteLine("OLE Object Source Full Name: " + oleObject.ObjectSourceFullName);

            // Сохраните книгу
            workbook.Save("OleObjectDemo.xlsx");
        }
    }
}
```

### См. также

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


