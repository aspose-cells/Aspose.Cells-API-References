---
title: "Classe ConditionalFormattingIcon"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.ConditionalFormattingIcon. Rappresenta l'icona personalizzata della regola di formattazione condizionale"
type: docs
url: /it/net/aspose.cells/conditionalformattingicon/
---
## ConditionalFormattingIcon class

Rappresenta l'icona personalizzata della regola di formattazione condizionale.

```csharp
public class ConditionalFormattingIcon
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ImageData](../../aspose.cells/conditionalformattingicon/imagedata/) { get; } | Ottiene i dati del set di icone. |
| [Index](../../aspose.cells/conditionalformattingicon/index/) { get; set; } | Ottiene e imposta l'indice dell'icona nel set di icone. |
| [Type](../../aspose.cells/conditionalformattingicon/type/) { get; set; } | Ottiene e imposta il tipo di set di icone. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetImageData](../../aspose.cells/conditionalformattingicon/getimagedata/)(Cell) | Ottiene i dati dell'immagine con l'impostazione della cella. |
| static [GetIconImageData](../../aspose.cells/conditionalformattingicon/geticonimagedata/)(IconSetType, int) | Ottieni i dati del set di icone |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingIconDemo
    {
        public static void ConditionalFormattingIconExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro nella cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ottieni la collezione Conditional Formattings
            ConditionalFormattingCollection cformattings = worksheet.ConditionalFormattings;
            
            // Aggiungi una nuova formattazione condizionale alla raccolta
            int index = cformattings.Add();
            
            // Accedi alla raccolta di condizioni di formattazione
            FormatConditionCollection fcs = cformattings[index];
            
            // Definisci l'area di celle a cui applicare la formattazione condizionale
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 0
            };
            
            // Aggiungi l'area di celle alla raccolta di condizioni di formattazione
            fcs.AddArea(ca);
            
            // Aggiungi una condizione per utilizzare i set di icone
            int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition fc = fcs[conditionIndex];
            
            // Imposta il tipo di set di icone
            fc.IconSet.Type = IconSetType.Arrows3;

            // Personalizza le icone individuali all'interno del set di icone
            ConditionalFormattingIcon cfIcon0 = fc.IconSet.CfIcons[0];
            cfIcon0.Type = IconSetType.Arrows3;
            cfIcon0.Index = 0;

            ConditionalFormattingIcon cfIcon1 = fc.IconSet.CfIcons[1];
            cfIcon1.Type = IconSetType.ArrowsGray3;
            cfIcon1.Index = 1;

            ConditionalFormattingIcon cfIcon2 = fc.IconSet.CfIcons[2];
            cfIcon2.Type = IconSetType.Boxes5;
            cfIcon2.Index = 2;

            // Salva la cartella di lavoro
            workbook.Save("ConditionalFormattingIconExample.xlsx");
            workbook.Save("ConditionalFormattingIconExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


