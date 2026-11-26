---
title: "Интерфейс IExportObjectListener"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Интерфейс Aspose.Cells.IExportObjectListener. Позволяет пользователям манипулировать объектами во время экспорта"
type: docs
url: /ru/net/aspose.cells/iexportobjectlistener/
---
## IExportObjectListener interface

Позволяет пользователям манипулировать объектами во время экспорта.

```csharp
public interface IExportObjectListener
```

## Методы

| Имя | Описание |
| --- | --- |
| [ExportObject](../../aspose.cells/iexportobjectlistener/exportobject/)(ExportObjectEvent) | Экспортировать один объект. |

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CellsClassIExportObjectListenerDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте пример изображения на лист
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.png");
            Picture picture = worksheet.Pictures[pictureIndex];
            
            // Реализация пользовательского слушателя экспорта
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportObjectListener = new CustomExportObjectListener();
            
            // Сохранить в HTML с пользовательским слушателем
            workbook.Save("output.html", saveOptions);
        }
    }

    class CustomExportObjectListener : IExportObjectListener
    {
        private int imgIdx = 0;
        
        public object ExportObject(ExportObjectEvent e)
        {
            object source = e.GetSource();
            if (source is Shape)
            {
                Shape shape = (Shape)source;
                if (shape.MsoDrawingType == MsoDrawingType.Picture)
                {
                    string url = SaveImage(((Picture)shape).Data, imgIdx, ((Picture)shape).ImageType);
                    imgIdx++;
                    return url;
                }
            }
            return null;
        }
        
        private string SaveImage(byte[] data, int imgIdx, ImageType format)
        {
            // В реальной реализации здесь вы бы сохраняли изображение на диск
            // Для демонстрационных целей мы просто возвращаем фиктивный путь
            return $"images/image_{imgIdx}.png";
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


