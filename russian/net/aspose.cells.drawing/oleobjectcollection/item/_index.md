---
title: "OleObjectCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство OleObjectCollection. Получает элемент OleObject по указанному индексу"
type: docs
url: /ru/net/aspose.cells.drawing/oleobjectcollection/item/
---
## OleObjectCollection indexer

Получает элемент [`OleObject`](../../oleobject/) по указанному индексу.

```csharp
public OleObject this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс элемента, начиная с нуля. |

### Возвращаемое значение

Элемент по указанному индексу.

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить образец данных изображения
            byte[] binaryImg = File.ReadAllBytes("image1.png");
            
            // Добавить OLE-объект в первый лист
            int idxOle = workbook.Worksheets[0].OleObjects.Add(0, 0, 60, 60, binaryImg);
            
            // Получить доступ к OLE-объекту с помощью свойства Item
            OleObject objOle = workbook.Worksheets[0].OleObjects[idxOle];
            
            // Установить свойства встроенного объекта
            byte[] binaryXlsx = File.ReadAllBytes("example.xlsx");
            objOle.SetEmbeddedObject(false, binaryXlsx, "SampleFile.xlsx", true, "Excel.Sheet", false);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
            
            // Проверьте сохранённый файл
            Workbook savedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("OLE Object Source: " + savedWorkbook.Worksheets[0].OleObjects[0].ObjectSourceFullName);
        }
    }
}
```

### См. также

* class [OleObject](../../oleobject/)
* class [OleObjectCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


