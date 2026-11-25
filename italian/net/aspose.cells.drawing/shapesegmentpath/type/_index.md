---
title: "ShapeSegmentPath.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ShapeSegmentPath. Ottiene il tipo del segmento del percorso"
type: docs
url: /it/net/aspose.cells.drawing/shapesegmentpath/type/
---
## ShapeSegmentPath.Type property

Ottiene il tipo di segmento del percorso

```csharp
public ShapePathType Type { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeSegmentPathPropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                //Crea un nuovo percorso di forma
                ShapePath shapePath = new ShapePath();

                // Sposta al punto di partenza
                shapePath.MoveTo(10, 10);

                // Chiama il metodo LineTo con parametri (Single, Single)
                shapePath.LineTo(50.5f, 10.5f);
                shapePath.LineTo(50.5f, 50.5f);
                shapePath.LineTo(10.5f, 50.5f);
                shapePath.Close();

                // Accedi alla proprietà PathSegementList
                ShapeSegmentPathCollection segmentList = shapePath.PathSegementList;

                // Visualizza il conteggio dei segmenti del percorso
                Console.WriteLine("Number of path segments: " + segmentList.Count);

                // Itera attraverso ogni segmento e visualizza il suo tipo
                foreach (ShapeSegmentPath segment in segmentList)
                {
                    Console.WriteLine("Segment type: " + segment.Type);
                }

                //aggiungi forma libera
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });

            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing LineTo method: {ex.Message}");
            }


            // Salva la cartella di lavoro
            workbook.Save("ShapeSegmentPathTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ShapePathType](../../shapepathtype/)
* class [ShapeSegmentPath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


