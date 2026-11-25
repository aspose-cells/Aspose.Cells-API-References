---
title: "FillFormat.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FillFormat. Ottiene e imposta il tipo di riempimento"
type: docs
url: /it/net/aspose.cells.drawing/fillformat/type/
---
## FillFormat.Type property

Ottiene e imposta il tipo di riempimento.

```csharp
[Obsolete("Use FillFormat.FillType  instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public FillType Type { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà FillFormat.FillType. Questa proprietà sarà rimossa 12 mesi dopo, a partire da luglio 2016. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class FillFormatPropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 200);
            FillFormat fill = shape.Fill;

            // Visualizza il valore corrente di Type
            Console.WriteLine("Current Type value: " + fill.Type);

            // Modifica Type in Gradient (proprietà obsoleta usata per la dimostrazione)
            fill.Type = FillType.Gradient;

            // Applica effetto gradiente a due colori
            fill.SetTwoColorGradient(Color.Blue, Color.Green, GradientStyleType.Horizontal, 1);

            // Salva la cartella di lavoro modificata
            workbook.Save("FillFormatTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [FillType](../../filltype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


