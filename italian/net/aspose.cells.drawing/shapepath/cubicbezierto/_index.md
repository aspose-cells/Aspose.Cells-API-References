---
title: "ShapePath.CubicBezierTo"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapePath. Aggiunge una curva Bézier cubica alla figura corrente. Il punto di partenza è il punto finale della figura corrente. Unità Pixel"
type: docs
url: /it/net/aspose.cells.drawing/shapepath/cubicbezierto/
---
## ShapePath.CubicBezierTo method

Aggiunge una curva Bézier cubica alla figura corrente. Il punto di partenza è il punto finale della figura corrente. Unità: Pixel.

```csharp
public void CubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, 
    float endY)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ctrX1 | Single | La coordinata x del primo punto di controllo della curva (Unit: Pixel). |
| ctrY1 | Single | La coordinata y del primo punto di controllo della curva (Unit: Pixel). |
| ctrX2 | Single | La coordinata x del secondo punto di controllo della curva (Unit: Pixel). |
| ctrY2 | Single | La coordinata y del secondo punto di controllo della curva (Unit: Pixel). |
| endX | Single | La coordinata x del punto finale della curva (Unit: Pixel). |
| endY | Single | La coordinata y del punto finale della curva (Unit: Pixel). |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodCubicBezierToWithSingleSingleSingleSingleSingleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            //Crea un nuovo percorso di forma
            ShapePath shapePath1 = new ShapePath();
            shapePath1.MoveTo(0, 0);
            shapePath1.CubicBezierTo(48.24997f, 0.6844f,
                        96.5f, -7.148871f,
                        130, 11.517795f);
            shapePath1.CubicBezierTo(163.5f, 30.18446f,
                        182.24997f, 75.351f,
                        201, 120.517795f);
            shapePath1.MoveTo(150, 70);
            shapePath1.ArcTo(25, 25, 0, 270);


            //aggiungi forma libera
            worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath1 });

            // Salva il risultato
            workbook.Save("ShapePathMethodCubicBezierToDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


