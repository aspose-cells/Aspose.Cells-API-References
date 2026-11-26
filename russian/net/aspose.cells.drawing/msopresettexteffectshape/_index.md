---
title: "Перечисление MsoPresetTextEffectShape"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.MsoPresetTextEffectShape. Представляет тип предустановленной формы текстового эффекта WordArt"
type: docs
url: /ru/net/aspose.cells.drawing/msopresettexteffectshape/
---
## MsoPresetTextEffectShape enumeration

Представляет тип предустановленной формы текстового эффекта WordArt.

```csharp
public enum MsoPresetTextEffectShape
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| PlainText | `136` | ПростойТекст |
| Stop | `137` | Стоп |
| TriangleUp | `138` | ТреугольникВверх |
| TriangleDown | `139` | ТреугольникВниз |
| ChevronUp | `140` | ШевронВверх |
| ChevronDown | `141` | ШевронВниз |
| RingInside | `142` | КольцоВнутри |
| RingOutside | `143` | КольцоСнаружи |
| ArchUpCurve | `144` | АркаВверхКривая |
| ArchDownCurve | `145` | АркаВнизКривая |
| CircleCurve | `146` | КруговаяКривая |
| ButtonCurve | `147` | КнопкаКривая |
| ArchUpPour | `148` | АркаВверхЗаливка |
| ArchDownPour | `149` | АркаВнизЗаливка |
| CirclePour | `150` | КругЗаливка |
| ButtonPour | `151` | КнопкаЗаливка |
| CurveUp | `152` | КриваяВверх |
| CurveDown | `153` | КриваяВниз |
| CanUp | `174` | БанкаВверх |
| CanDown | `175` | БанкаВниз |
| Wave1 | `156` | Волна1 |
| Wave2 | `157` | Волна2 |
| DoubleWave1 | `158` | ДвойнаяВолна1 |
| DoubleWave2 | `159` | ДвойнаяВолна2 |
| Inflate | `160` | Надуть |
| Deflate | `161` | Сжать |
| InflateBottom | `162` | Развернуть снизу |
| DeflateBottom | `163` | Сжать снизу |
| InflateTop | `164` | Развернуть сверху |
| DeflateTop | `165` | Сжать сверху |
| DeflateInflate | `166` | СжатьРазвернуть |
| DeflateInflateDeflate | `167` | СжатьРазвернутьСжать |
| FadeRight | `168` | Затухание вправо |
| FadeLeft | `169` | Затухание влево |
| FadeUp | `170` | Затухание вверх |
| FadeDown | `171` | Затухание вниз |
| SlantUp | `172` | Наклон вверх |
| SlantDown | `173` | Наклон вниз |
| CascadeUp | `154` | Каскад вверх |
| CascadeDown | `155` | Каскад вниз |
| Mixed | `255` | Смешанный |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoPresetTextEffectShapeDemo
    {
        public static void MsoPresetTextEffectShapeExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // Добавление формы текстового эффекта WordArt
            shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Aspose", "Arial", 30, false, false, 0, 0, 0, 0, 100, 200);
            TextEffectFormat textEffectFormat = shapes[0].TextEffect;

            // Установка предустановленного типа формы
            textEffectFormat.PresetShape = MsoPresetTextEffectShape.ArchUpCurve;

            // Сохраните книгу
            workbook.Save("MsoPresetTextEffectShapeExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


