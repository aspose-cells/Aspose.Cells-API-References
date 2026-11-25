---
title: "ShapeCollection.AddCopy"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ShapeCollection metodo. Aggiunge e copia una forma al foglio di lavoro"
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/addcopy/
---
## AddCopy(Shape, int, int, int, int) {#addcopy}

Aggiunge e copia una forma al foglio di lavoro.

```csharp
public Shape AddCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceShape | Forma | Forma sorgente. |
| topRow | Int32 | L'indice della riga superiore. |
| alto | Int32 | Rappresenta lo spostamento verticale dalla sua riga superiore, in unità di pixel. |
| leftColumn | Int32 | L'indice della colonna sinistra. |
| sinistra | Int32 | Rappresenta lo spostamento orizzontale dalla sua colonna sinistra, in unità di pixel. |

### Valore di ritorno

Il nuovo [`Shape`](../../shape/) oggetto.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddCopyWithShapeInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ottieni la collezione di forme
            ShapeCollection shapes = worksheet.Shapes;

            // Aggiungi una forma rettangolare
            RectangleShape rectangle = shapes.AddRectangle(2, 0, 2, 0, 130, 130);

            // Aggiungi una copia della forma rettangolare con nuova posizione
            shapes.AddCopy(rectangle, 7, 0, 7, 0);

            // Salva la cartella di lavoro
            workbook.Save("ShapeCollectionMethodAddCopyDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## AddCopy(Shape, int, int, int, int, CopyOptions) {#addcopy_1}

Aggiunge e copia una forma al foglio di lavoro.

```csharp
public Shape AddCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left, 
    CopyOptions copyOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceShape | Forma | Forma sorgente. |
| topRow | Int32 | L'indice della riga superiore. |
| alto | Int32 | Rappresenta lo spostamento verticale dalla sua riga superiore, in unità di pixel. |
| leftColumn | Int32 | L'indice della colonna sinistra. |
| sinistra | Int32 | Rappresenta lo spostamento orizzontale dalla sua colonna sinistra, in unità di pixel. |
| copyOptions | CopyOptions | Le opzioni di copia delle forme. |

### Valore di ritorno

Il nuovo [`Shape`](../../shape/) oggetto.

### Esempi

```csharp

[C#]
//aggiungi una forma
RectangleShape rectangle = shapes.AddRectangle(2, 0, 2, 0, 130, 130);
//Aggiunge e copia una forma.
shapes.AddCopy(rectangle, 7, 0, 7, 0);
```

### Vedi anche

* class [Shape](../../shape/)
* class [CopyOptions](../../../aspose.cells/copyoptions/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


