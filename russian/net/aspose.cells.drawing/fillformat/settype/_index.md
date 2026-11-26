---
title: "FillFormat.SetType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FillFormat. Получает тип установленного формата заливки"
type: docs
url: /ru/net/aspose.cells.drawing/fillformat/settype/
---
## FillFormat.SetType property

Получает тип установленного формата заливки.

```csharp
[Obsolete("Use FillFormat.FillType instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public FormatSetType SetType { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство FillFormat.FillType. Это свойство будет удалено через 12 месяцев, начиная с июля 2016 года. Aspose извиняется за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class FillFormatPropertySetTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 200, 200);
            FillFormat fillFormat = shape.Fill;

            Console.WriteLine("Current SetType value: " + fillFormat.SetType);

            fillFormat.SetType = FormatSetType.IsGradientSet;
            fillFormat.SetTwoColorGradient(Color.LightBlue, Color.DarkBlue, GradientStyleType.Horizontal, 1);

            Console.WriteLine("New SetType value: " + fillFormat.SetType);

            workbook.Save("FillFormatSetTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [FormatSetType](../../formatsettype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


