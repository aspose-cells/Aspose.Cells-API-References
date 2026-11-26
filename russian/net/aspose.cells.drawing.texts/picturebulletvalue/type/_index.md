---
title: "PictureBulletValue.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PictureBulletValue. Получает тип значения маркера"
type: docs
url: /ru/net/aspose.cells.drawing.texts/picturebulletvalue/type/
---
## PictureBulletValue.Type property

Получает тип значения маркера.

```csharp
public override BulletType Type { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class PictureBulletValuePropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Создайте экземпляр PictureBulletValue
                PictureBulletValue bulletValue = new PictureBulletValue();
                
                // Отобразить значение свойства Type (операция только для чтения)
                Console.WriteLine("PictureBulletValue Type: " + bulletValue.Type);
                
                // Продемонстрировать, что свойство Type правильно установлено в Picture для этого класса
                if (bulletValue.Type == BulletType.Picture)
                {
                    Console.WriteLine("Type is correctly set to Picture for PictureBulletValue");
                }
                
                // Сохраните книгу
                workbook.Save("PictureBulletValueTypeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [BulletType](../../bullettype/)
* class [PictureBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


