---
title: "Shape.AddHyperlink"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Shape. Aggiunge un collegamento ipertestuale alla forma"
type: docs
url: /it/net/aspose.cells.drawing/shape/addhyperlink/
---
## Shape.AddHyperlink method

Aggiunge un collegamento ipertestuale alla forma.

```csharp
public Hyperlink AddHyperlink(string address)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| address | String | Indirizzo del collegamento ipertestuale. |

### Valore di ritorno

Restituisce il nuovo oggetto collegamento ipertestuale.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodAddHyperlinkWithStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma al foglio di lavoro
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Aggiungi un collegamento ipertestuale alla forma usando una stringa URL
            Aspose.Cells.Hyperlink hyperlink = shape.AddHyperlink("https://www.aspose.com/");

            // Salva la cartella di lavoro
            workbook.Save("ShapeWithHyperlink.xlsx");
        }
    }
}
```

### Vedi anche

* class [Hyperlink](../../../aspose.cells/hyperlink/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


