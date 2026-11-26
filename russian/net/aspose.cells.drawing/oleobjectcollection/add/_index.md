---
title: "OleObjectCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод OleObjectCollection. Добавляет OleObject в коллекцию"
type: docs
url: /ru/net/aspose.cells.drawing/oleobjectcollection/add/
---
## Add(int, int, int, int, byte[]) {#add}

Добавляет OleObject в коллекцию.

```csharp
public int Add(int topRow, int leftColumn, int height, int width, byte[] imageData)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | Int32 | Индекс строки в верхнем левом углу. |
| leftColumn | Int32 | Индекс столбца в верхнем левом углу. |
| высота | Int32 | Высота oleObject в пикселях. |
| ширина | Int32 | Ширина oleObject в пикселях. |
| imageData | Byte[] | Изображение oleObject в виде массива байтов. |

### Возвращаемое значение

[`OleObject`](../../oleobject/) object index.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class OleObjectCollectionMethodAddWithInt32Int32Int32Int32ByteDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Подготовьте данные OLE-объекта (пример файла Excel в виде массива байтов)
            byte[] oleData;
            try
            {
                string sampleFilePath = "sample.xlsx";
                oleData = File.ReadAllBytes(sampleFilePath);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error reading sample file: {ex.Message}");
                return;
            }

            try
            {
                // Вызовите метод Add с параметрами: (upperLeftRow, upperLeftColumn, height, width, imageData)
                int oleIndex = worksheet.OleObjects.Add(5, 2, 200, 300, oleData);

                Console.WriteLine($"OLE object added successfully at index: {oleIndex}");
                Console.WriteLine($"Position: Row 5, Column 2");
                Console.WriteLine($"Size: 200px height, 300px width");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("OleObjectAddDemo.xlsx");
        }
    }
}
```

### См. также

* class [OleObjectCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, int, int, byte[], string) {#add_1}

Добавляет связанный OleObject в коллекцию.

```csharp
public int Add(int topRow, int leftColumn, int height, int width, byte[] imageData, 
    string linkedFile)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | Int32 | Индекс строки в верхнем левом углу. |
| leftColumn | Int32 | Индекс столбца в верхнем левом углу. |
| высота | Int32 | Высота oleObject в пикселях. |
| ширина | Int32 | Ширина oleObject в пикселях. |
| imageData | Byte[] | Изображение oleObject в виде массива байтов. |
| linkedFile | String |  |

### Возвращаемое значение

[`OleObject`](../../oleobject/) object index.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class OleObjectCollectionMethodAddWithInt32Int32Int32Int32ByteStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Подготовьте данные OLE-объекта
            int upperLeftRow = 1;
            int upperLeftColumn = 1;
            int height = 200;
            int width = 200;
            byte[] imageData = File.ReadAllBytes("sample.ole");
            string linkedFile = "sample.xlsx";

            try
            {
                // Вызовите метод Add с конкретными типами параметров
                int index = worksheet.OleObjects.Add(upperLeftRow, upperLeftColumn, height, width, imageData, linkedFile);
                
                Console.WriteLine($"OLE object added at index: {index}");
                Console.WriteLine($"Total OLE objects in worksheet: {worksheet.OleObjects.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("OleObjectAddDemo.xlsx");
        }
    }
}
```

### См. также

* class [OleObjectCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


