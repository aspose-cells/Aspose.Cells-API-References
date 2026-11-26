---
title: "Перечисление ControlPicturePositionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.ActiveXControls.ControlPicturePositionType. Представляет расположение изображения элемента управления относительно его подписи"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/controlpicturepositiontype/
---
## ControlPicturePositionType enumeration

Представляет расположение изображения элемента управления относительно его подписи.

```csharp
public enum ControlPicturePositionType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| LeftTop | `131072` | Изображение расположено слева от подписи. Подпись выровнена по верхнему краю изображения. |
| LeftCenter | `327683` | Изображение расположено слева от подписи. Подпись центрирована относительно изображения. |
| LeftBottom | `524294` | Изображение расположено слева от подписи. Подпись выровнена по нижнему краю изображения. |
| RightTop | `2` | Изображение расположено справа от подписи. Подпись выровнена по верхнему краю изображения. |
| RightCenter | `196613` | Изображение расположено справа от подписи. Подпись центрирована относительно изображения. |
| RightBottom | `393224` | Изображение расположено справа от подписи. Подпись выровнена по нижнему краю изображения. |
| AboveLeft | `393216` | Изображение расположено над подписью. Подпись выровнена по левому краю изображения. |
| AboveCenter | `458753` | Изображение расположено над подписью. Подпись центрирована под изображением. |
| AboveRight | `524290` | Изображение расположено над подписью. Подпись выровнена по правому краю изображения. |
| BelowLeft | `6` | Изображение расположено под подписью. Подпись выровнена по левому краю изображения. |
| BelowCenter | `65543` | Изображение расположено под подписью. Подпись центрирована над изображением. |
| BelowRight | `131080` | Изображение расположено под подписью. Подпись выровнена по правому краю изображения. |
| Center | `262148` | Изображение расположено в центре элемента управления. Подпись центрирована по горизонтали и вертикали над изображением. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlsClassControlPicturePositionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Shape shape = workbook.Worksheets[0].Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 0, 1, 0, 100, 50);
            ToggleButtonActiveXControl activeXControl = (ToggleButtonActiveXControl)shape.ActiveXControl;

            activeXControl.Caption = "Demo Button";
            activeXControl.PicturePosition = ControlPicturePositionType.AboveLeft;
            activeXControl.IsAutoSize = true;

            workbook.Save("ActiveXControlDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


