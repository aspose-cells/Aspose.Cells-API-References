---
title: "Enum MsoPresetTextEffectShape"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.Drawing.MsoPresetTextEffectShape. Representa el tipo de forma de efecto de texto predefinido de WordArt"
type: docs
url: /es/net/aspose.cells.drawing/msopresettexteffectshape/
---
## MsoPresetTextEffectShape enumeration

Representa el tipo de forma de efecto de texto preestablecido de WordArt.

```csharp
public enum MsoPresetTextEffectShape
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| PlainText | `136` | TextoPlano |
| Stop | `137` | Detener |
| TriangleUp | `138` | TriánguloArriba |
| TriangleDown | `139` | TriánguloAbajo |
| ChevronUp | `140` | ChevronArriba |
| ChevronDown | `141` | ChevronAbajo |
| RingInside | `142` | AnilloInterior |
| RingOutside | `143` | AnilloExterior |
| ArchUpCurve | `144` | ArcoArribaCurva |
| ArchDownCurve | `145` | ArcoAbajoCurva |
| CircleCurve | `146` | CírculoCurva |
| ButtonCurve | `147` | BotónCurva |
| ArchUpPour | `148` | ArcoArribaVertido |
| ArchDownPour | `149` | ArcoAbajoVertido |
| CirclePour | `150` | CírculoVertido |
| ButtonPour | `151` | BotónVertido |
| CurveUp | `152` | CurvaArriba |
| CurveDown | `153` | CurvaAbajo |
| CanUp | `174` | LataArriba |
| CanDown | `175` | LataAbajo |
| Wave1 | `156` | Ola1 |
| Wave2 | `157` | Ola2 |
| DoubleWave1 | `158` | DobleOla1 |
| DoubleWave2 | `159` | DobleOla2 |
| Inflate | `160` | Inflar |
| Deflate | `161` | Deflate |
| InflateBottom | `162` | InflateBottom |
| DeflateBottom | `163` | DeflateBottom |
| InflateTop | `164` | InflateTop |
| DeflateTop | `165` | DeflateTop |
| DeflateInflate | `166` | DeflateInflate |
| DeflateInflateDeflate | `167` | DeflateInflateDeflate |
| FadeRight | `168` | FadeRight |
| FadeLeft | `169` | FadeLeft |
| FadeUp | `170` | FadeUp |
| FadeDown | `171` | FadeDown |
| SlantUp | `172` | SlantUp |
| SlantDown | `173` | SlantDown |
| CascadeUp | `154` | CascadeUp |
| CascadeDown | `155` | CascadeDown |
| Mixed | `255` | Mixed |

### Ejemplos

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
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // Agregar una forma de efecto de texto WordArt
            shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Aspose", "Arial", 30, false, false, 0, 0, 0, 0, 100, 200);
            TextEffectFormat textEffectFormat = shapes[0].TextEffect;

            // Estableciendo el tipo de forma predefinido
            textEffectFormat.PresetShape = MsoPresetTextEffectShape.ArchUpCurve;

            // Guarda el libro de trabajo
            workbook.Save("MsoPresetTextEffectShapeExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


