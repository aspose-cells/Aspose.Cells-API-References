---
title: "UnknownControl.Data"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство UnknownControl. Получает и задает двоичные данные контролла"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/unknowncontrol/data/
---
## UnknownControl.Data property

Получает и задает двоичные данные элемента управления.

```csharp
public override byte[] Data { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class UnknownControlPropertyDataDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте фиктивный CLSID (недействительный идентификатор)
            byte[] dummyClsid = new byte[16];

            // Добавьте неизвестный ActiveX‑контролл, используя ControlType.Unknown с полными параметрами
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.Unknown, 0, 0, 100, 100, 0, 0);

            // Получите доступ к экземпляру UnknownControl
            UnknownControl unknownControl = (UnknownControl)shape.ActiveXControl;

            // Установите данные контролла, включая CLSID, копируя их в существующий массив
            Array.Copy(dummyClsid, unknownControl.Data, dummyClsid.Length);

            // Прочитайте и отобразите информацию свойства Data
            Console.WriteLine($"Unknown control data length: {unknownControl.Data.Length}");
            Console.WriteLine($"Control type: {unknownControl.Type}");

            // Продемонстрировать сохранение данных управления в выходном файле
            workbook.Save("UnknownControlDataDemo.xlsx");
        }
    }
}
```

### См. также

* class [UnknownControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


