---
title: "MsoFillFormat.IsVisible"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MsoFillFormat. Indica se è presente un riempimento"
type: docs
url: /it/net/aspose.cells.drawing/msofillformat/isvisible/
---
## MsoFillFormat.IsVisible property

Indica se è presente un riempimento.

```csharp
public bool IsVisible { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFillFormatPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una forma di esempio
            Shape shape1 = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
            Shape shape2 = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 100, 150);

            // Imposta la visibilità del riempimento per shape1 (visibile)
            shape1.FillFormat.IsVisible = true;
            shape1.FillFormat.ForeColor = System.Drawing.Color.Red;
            
            // Imposta la visibilità del riempimento per shape2 (invisibile)
            shape2.FillFormat.IsVisible = false;

            // Dimostra l'uso della proprietà IsVisible
            Console.WriteLine("Shape1 Fill Visible: " + shape1.FillFormat.IsVisible);
            Console.WriteLine("Shape2 Fill Visible: " + shape2.FillFormat.IsVisible);

            // Confronta la visibilità del riempimento tra le forme
            if (shape1.FillFormat.IsVisible && shape2.FillFormat.IsVisible)
            {
                Console.WriteLine("Both shapes have visible fills");
            }
            else
            {
                Console.WriteLine("At least one shape has invisible fill");
            }

            // Salva la cartella di lavoro
            workbook.Save("MsoFillFormatIsVisibleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


