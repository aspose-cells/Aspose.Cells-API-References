---
title: "Shape.LineFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Restituisce un oggetto MsoLineFormat che contiene le proprietà di formattazione della linea per la forma specificata"
type: docs
url: /it/net/aspose.cells.drawing/shape/lineformat/
---
## Shape.LineFormat property

Restituisce un oggetto MsoLineFormat che contiene le proprietà di formattazione della linea per la forma specificata.

```csharp
[Obsolete("Use Shape.Line property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MsoLineFormat LineFormat { get; }
```

### Osservazioni

NOTA: questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Shape.Line. Questa proprietà sarà rimossa 12 mesi dopo, a partire da luglio 2016. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLineFormatDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi una forma rettangolare al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            RectangleShape rectangle = worksheet.Shapes.AddRectangle(3, 0, 2, 0, 70, 130);
            
            // Imposta le proprietà della forma
            rectangle.Placement = PlacementType.FreeFloating;
            rectangle.Fill.FillType = FillType.Solid;
            rectangle.Fill.SolidFill.Color = System.Drawing.Color.Blue;
            
            // Dimostra l'uso di LineFormat
            rectangle.LineFormat.Weight = 3; // Set line weight
            rectangle.LineFormat.DashStyle = MsoLineDashStyle.Solid;
            rectangle.Line.SolidFill.Color = System.Drawing.Color.DarkBlue; // Correct way to set line color
            
            // Salva la cartella di lavoro
            workbook.Save("ShapeLineFormatDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [MsoLineFormat](../../msolineformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


