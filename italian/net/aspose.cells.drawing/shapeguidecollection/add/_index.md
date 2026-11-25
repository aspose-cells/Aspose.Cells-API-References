---
title: "ShapeGuideCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapeGuideCollection. Aggiunge una guida di forma. Importante: questa funzionalità è attualmente disponibile solo per Excel07 e versioni successive"
type: docs
url: /it/net/aspose.cells.drawing/shapeguidecollection/add/
---
## ShapeGuideCollection.Add method

Aggiunge una guida di forma.(Importante: questa funzionalità è attualmente disponibile solo per Excel07 e versioni successive)

```csharp
public int Add(string name, double val)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | il nome di adjust. È così "adj (Usato quando c'è un solo valore di regolazione)", "adj1", "adj2", "adj3" e così via. |
| val | Double | il valore di adjust |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeGuideCollectionMethodAddWithStringDoubleDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una forma che utilizza guide di regolazione
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.RightArrowCallout, 2, 0, 2, 0, 200, 150);

            try
            {
                // Ottieni lo ShapeGuideCollection dalle regolazioni della geometria della forma
                ShapeGuideCollection shapeGuides = shape.Geometry.ShapeAdjustValues;

                // Chiama il metodo Add con parametri (String, Double)
                shapeGuides.Add("adj1", 25.5);
                shapeGuides.Add("adj2", 25.5);
                shapeGuides.Add("adj3", 25.5);
                shapeGuides.Add("adj4", 25.5);

                Console.WriteLine($"Total guides after addition: {shapeGuides.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }

            // Salva la cartella di lavoro modificata
            workbook.Save("ShapeGuideAddWithStringDoubleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ShapeGuideCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


