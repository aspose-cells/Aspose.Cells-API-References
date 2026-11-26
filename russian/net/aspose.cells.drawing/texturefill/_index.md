---
title: "Класс TextureFill"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.TextureFill. Инкапсулирует объект, представляющий формат заливки текстурой"
type: docs
url: /ru/net/aspose.cells.drawing/texturefill/
---
## TextureFill class

Инкапсулирует объект, представляющий формат текстурной заливки.

```csharp
public class TextureFill : Fill
```

## Свойства

| Имя | Описание |
| --- | --- |
| [ImageData](../../aspose.cells.drawing/texturefill/imagedata/) { get; set; } | Получает и задает данные изображения заливки. |
| [IsTiling](../../aspose.cells.drawing/texturefill/istiling/) { get; set; } | Указывает, использовать ли изображение плиткой в качестве текстуры. |
| [PicFormatOption](../../aspose.cells.drawing/texturefill/picformatoption/) { get; set; } | Получает или задает параметр формата изображения. |
| [PictureFormatType](../../aspose.cells.drawing/texturefill/pictureformattype/) { get; set; } | Получает и задает тип формата изображения. |
| [Scale](../../aspose.cells.drawing/texturefill/scale/) { get; set; } | Получает и задает масштаб формата изображения. |
| [TilePicOption](../../aspose.cells.drawing/texturefill/tilepicoption/) { get; set; } | Получает или задает параметр мозаичной картинки. |
| [Transparency](../../aspose.cells.drawing/texturefill/transparency/) { get; set; } | Возвращает или задает степень прозрачности области значением от 0.0 (непрозрачный) до 1.0 (прозрачный). |
| [Type](../../aspose.cells.drawing/texturefill/type/) { get; set; } | Получает и задает тип текстуры |

## Методы

| Имя | Описание |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(Унаследовано от [`Fill`](../fill/).) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Получает хеш-код.(Унаследовано от [`Fill`](../fill/).) |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassTextureFillDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте прямоугольную форму, чтобы продемонстрировать заливку текстурой
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 150, 300);
            
            // Примените заливку текстурой к форме и получите существующий экземпляр TextureFill
            shape.Fill.FillType = FillType.Texture;
            TextureFill textureFill = shape.Fill.TextureFill;
            
            // Установите встроенный тип текстуры
            textureFill.Type = TextureType.BlueTissuePaper;
            
            // Настройте параметры мозаики
            textureFill.IsTiling = true;
            TilePicOption tileOptions = new TilePicOption
            {
                ScaleX = 0.5,
                ScaleY = 0.5,
                OffsetX = 10,
                OffsetY = 10
            };
            textureFill.TilePicOption = tileOptions;
            
            // Установите прозрачность заливки и масштабирование
            textureFill.Transparency = 0.2;
            textureFill.Scale = 0.8;
            
            // Сохраните книгу с применённой заливкой текстурой
            workbook.Save("TextureFillDemo.xlsx");
        }
    }
}
```

### См. также

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


