---
title: "ShapePath.ArcTo"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ShapePath metodo. Aggiunge un arco ellittico alla figura corrente. Il punto di partenza è il punto finale della figura corrente"
type: docs
url: /it/net/aspose.cells.drawing/shapepath/arcto/
---
## ShapePath.ArcTo method

Aggiunge un arco ellittico alla figura corrente. Il punto di partenza è il punto finale della figura corrente.

```csharp
public void ArcTo(float wR, float hR, float stAng, float swAng)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| wR | Single | La metà della larghezza dell'area rettangolare dell'ellisse che disegna l'arco (Unità: Pixel). |
| hR | Single | La metà dell'altezza dell'area rettangolare dell'ellisse che disegna l'arco (Unità: Pixel). |
| stAng | Single | L'angolo di partenza dell'arco, misurato in gradi in senso orario dall'asse x (Unità: Grado). Questo angolo specificherà quale angolo lungo il percorso circolare presunto verrà usato come posizione iniziale per disegnare l'arco. Questo angolo di partenza sarà bloccato all'ultima posizione nota della penna nel shape path. Garantendo così un shape path continuo. |
| swAng | Single | L'angolo di swing per un arco. Questo angolo specificherà fino a che punto, in termini di angolo, lungo il percorso circolare presunto l'arco sarà esteso. L'estensione dall'angolo di partenza sarà sempre nella direzione oraria attorno al cerchio presunto. (Unità: Grado) |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodArcToWithSingleSingleSingleSingleDemo
    {
        public static void Run()
        {
            //Crea un nuovo percorso di forma
            ShapePath shapePath = new ShapePath();
            shapePath.MoveTo(60, 45);
            shapePath.ArcTo(25, 25, 0, 270);
            shapePath.Close();

            shapePath.MoveTo(60, 20);
            shapePath.LineTo(110, 70);
            shapePath.LineTo(125, 155.5f);
            shapePath.ArcTo(35.5f, 35.5f, 0, 270);
            shapePath.Close();

            shapePath.MoveTo(150, 45);
            shapePath.ArcTo(25, 25, 0, 270);

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

            Workbook workbook = new Workbook();

            //aggiungi forma libera
            workbook.Worksheets[0].Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath, shapePath1 });

            // Salva il risultato
            workbook.Save("ShapePathMethodArcToDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


