---
title: "OleObject.IsLink"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство OleObject. Возвращает true, если OleObject ссылается на файл"
type: docs
url: /ru/net/aspose.cells.drawing/oleobject/islink/
---
## OleObject.IsLink property

Возвращает true, если OleObject ссылается на файл.

```csharp
public bool IsLink { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyIsLinkDemo
    {
        public static void Run()
        {
            // Загрузить исходную книгу
            Workbook workbook = new Workbook("example.xlsm");

            // Обработать каждый лист
            foreach (Worksheet worksheet in workbook.Worksheets)
            {
                // Обработать каждый OLE‑объект в листе
                foreach (Aspose.Cells.Drawing.OleObject ole in worksheet.OleObjects)
                {
                    // Пропустить, если OLE‑объект не связан
                    if (!ole.IsLink)
                    {
                        Console.WriteLine("Skipping embedded OLE object");
                        continue;
                    }

                    // Отобразить и изменить путь к связанному файлу
                    Console.WriteLine("Original linked file: " + ole.ObjectSourceFullName);
                    string newPath = ole.ObjectSourceFullName.Replace("C:", "D:");
                    ole.ObjectSourceFullName = newPath;
                    Console.WriteLine("Modified linked file: " + ole.ObjectSourceFullName);
                }
            }

            // Сохранить изменённую книгу
            workbook.Save("modified_example.xlsm");
            Console.WriteLine("File saved with updated OLE links.");
        }
    }
}
```

### См. также

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


