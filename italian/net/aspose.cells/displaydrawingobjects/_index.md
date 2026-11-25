---
title: "Enum DisplayDrawingObjects"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.DisplayDrawingObjects enum. Rappresenta se e come mostrare gli oggetti nella cartella di lavoro"
type: docs
url: /it/net/aspose.cells/displaydrawingobjects/
---
## DisplayDrawingObjects enumeration

Rappresenta se e come mostrare gli oggetti nella cartella di lavoro.

```csharp
public enum DisplayDrawingObjects
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| DisplayShapes | `0` | Mostra tutti gli oggetti |
| Placeholders | `1` | Mostra i segnaposto |
| Hide | `2` | Nascondi tutte le forme. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DisplayDrawingObjectsDemo
    {
        public static void DisplayDrawingObjectsExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi alle impostazioni della cartella di lavoro
            WorkbookSettings settings = workbook.Settings;

            // Imposta la proprietà DisplayDrawingObjects per mostrare tutti gli oggetti
            settings.DisplayDrawingObjects = DisplayDrawingObjects.DisplayShapes;

            // Salva la cartella di lavoro
            workbook.Save("DisplayDrawingObjectsExample_DisplayShapes.xlsx");

            // Imposta la proprietà DisplayDrawingObjects per mostrare i segnaposto
            settings.DisplayDrawingObjects = DisplayDrawingObjects.Placeholders;

            // Salva la cartella di lavoro
            workbook.Save("DisplayDrawingObjectsExample_Placeholders.xlsx");

            // Imposta la proprietà DisplayDrawingObjects per nascondere tutte le forme
            settings.DisplayDrawingObjects = DisplayDrawingObjects.Hide;

            // Salva la cartella di lavoro
            workbook.Save("DisplayDrawingObjectsExample_Hide.xlsx");
            workbook.Save("DisplayDrawingObjectsExample_Hide.pdf");
            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


