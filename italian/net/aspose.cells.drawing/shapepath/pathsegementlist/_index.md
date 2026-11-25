---
title: "ShapePath.PathSegementList"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ShapePath. Ottiene l'elenco ShapeSegmentPathCollection"
type: docs
url: /it/net/aspose.cells.drawing/shapepath/pathsegementlist/
---
## ShapePath.PathSegementList property

Ottiene l'elenco [`ShapeSegmentPathCollection`](../../shapesegmentpathcollection/)

```csharp
[Obsolete("Use ShapePath.PathSegments property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ShapeSegmentPathCollection PathSegementList { get; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà ShapePath.PathSegments. Questa proprietà sarà rimossa 12 mesi dopo, a partire da luglio 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPropertyPathSegementListDemo
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

                Console.WriteLine("MoveTo method executed successfully with parameters (Single, Single)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing LineTo method: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("ShapePathPropertyPathSegementListDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ShapeSegmentPathCollection](../../shapesegmentpathcollection/)
* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


