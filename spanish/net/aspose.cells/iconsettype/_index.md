---
title: "Enumeración IconSetType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.IconSetType. Tipo de conjunto de íconos para formato condicional. Los valores de umbral para activar los diferentes íconos dentro de un conjunto son configurables y el orden de los íconos es reversible"
type: docs
url: /es/net/aspose.cells/iconsettype/
---
## IconSetType enumeration

Tipo de conjunto de íconos para formato condicional. Los valores de umbral para activar los diferentes íconos dentro de un conjunto son configurables, y el orden de los íconos es reversible.

```csharp
public enum IconSetType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Arrows3 | `0` | Conjunto de íconos de 3 flechas. |
| ArrowsGray3 | `1` | Conjunto de íconos de 3 flechas grises. |
| Flags3 | `2` | Conjunto de íconos de 3 banderas. |
| Signs3 | `3` | Conjunto de íconos de 3 señales. |
| Symbols3 | `4` | Conjunto de íconos de 3 símbolos (con círculo). |
| Symbols32 | `5` | Conjunto de íconos de 3 símbolos (sin círculo). |
| TrafficLights31 | `6` | Conjunto de íconos de 3 semáforos (sin borde). |
| TrafficLights32 | `7` | Conjunto de íconos de 3 semáforos con borde negro grueso. |
| Arrows4 | `8` | Conjunto de íconos de 4 flechas. |
| ArrowsGray4 | `9` | Conjunto de íconos de 4 flechas grises. |
| Rating4 | `10` | Conjunto de íconos de 4 calificaciones. |
| RedToBlack4 | `11` | Conjunto de íconos de 4 'rojo a negro'. |
| TrafficLights4 | `12` | Conjunto de íconos de 4 semáforos. |
| Arrows5 | `13` | Conjunto de iconos de 5 flechas. |
| ArrowsGray5 | `14` | Conjunto de iconos de 5 flechas grises. |
| Quarters5 | `15` | Conjunto de iconos de 5 cuartos. |
| Rating5 | `16` | Conjunto de iconos de 5 calificaciones. |
| Stars3 | `17` | Conjunto de 3 estrellas |
| Boxes5 | `18` | Conjunto de 5 cajas |
| Triangles3 | `19` | Conjunto de 3 triángulos |
| None | `20` | Ninguno |
| CustomSet | `21` | CustomSet. Este elemento es de solo lectura. |
| Smilies3 | `22` | 3 emoticonos. Solo para .ods. |
| ColorSmilies3 | `23` | 3 emoticonos de color. Solo para .ods. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassIconSetTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Establecer valores de muestra
            cells["A1"].PutValue(1);
            cells["A2"].PutValue("#DIV/0!");
            cells["A3"].PutValue(3);

            // Agregar formato condicional con conjunto de iconos
            ConditionalFormattingCollection cfs = sheet.ConditionalFormattings;
            FormatConditionCollection fcs = cfs[cfs.Add()];
            fcs.AddArea(CellArea.CreateCellArea(0, 0, 3, 0));
            
            FormatCondition fc = fcs[fcs.AddCondition(FormatConditionType.IconSet)];
            fc.IconSet.Type = IconSetType.TrafficLights31;

            // Obtener y mostrar resultados
            ConditionalFormattingResult res1 = cells["A1"].GetConditionalFormattingResult();
            Console.WriteLine($"A1 Icon Type: {res1.ConditionalFormattingIcon.Type}, Index: {res1.ConditionalFormattingIcon.Index}");

            ConditionalFormattingResult res3 = cells["A3"].GetConditionalFormattingResult();
            Console.WriteLine($"A3 Icon Type: {res3.ConditionalFormattingIcon.Type}, Index: {res3.ConditionalFormattingIcon.Index}");

            ConditionalFormattingResult res2 = cells["A2"].GetConditionalFormattingResult();
            Console.WriteLine($"A2 has formatting: {res2 != null && res2.ConditionalFormattingIcon != null}");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


