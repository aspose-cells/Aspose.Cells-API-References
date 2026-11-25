---
title: "Classe FormatConditionCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.FormatConditionCollection. Rappresenta la formattazione condizionale. Le FormatConditions possono contenere fino a tre formati condizionali"
type: docs
url: /it/net/aspose.cells/formatconditioncollection/
---
## FormatConditionCollection class

Rappresenta la formattazione condizionale. Le FormatConditions possono contenere fino a tre formati condizionali.

```csharp
public class FormatConditionCollection
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.cells/formatconditioncollection/count/) { get; } | Ottiene il conteggio delle condizioni. |
| [Item](../../aspose.cells/formatconditioncollection/item/) { get; } | Ottiene la condizione di formattazione per indice. |
| [RangeCount](../../aspose.cells/formatconditioncollection/rangecount/) { get; } | Ottiene il conteggio degli intervalli formattati condizionalmente. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells/formatconditioncollection/add/)(CellArea, FormatConditionType, OperatorType, string, string) | Aggiunge una condizione di formattazione e l'intervallo di celle interessato alle FormatConditions. Le FormatConditions possono contenere fino a tre formati condizionali. I riferimenti ad altri fogli non sono consentiti nelle formule della formattazione condizionale. |
| [AddArea](../../aspose.cells/formatconditioncollection/addarea/)(CellArea) | Aggiunge un intervallo di celle formattato condizionalmente. |
| [AddCondition](../../aspose.cells/formatconditioncollection/addcondition/#addcondition)(FormatConditionType) | Aggiungi una condizione di formattazione. |
| [AddCondition](../../aspose.cells/formatconditioncollection/addcondition/#addcondition_1)(FormatConditionType, OperatorType, string, string) | Aggiunge una condizione di formattazione. |
| [GetCellArea](../../aspose.cells/formatconditioncollection/getcellarea/)(int) | Ottiene l'intervallo di celle formattato condizionalmente per indice. |
| [RemoveArea](../../aspose.cells/formatconditioncollection/removearea/#removearea_1)(int) | Rimuove l'intervallo di celle formattato condizionalmente per indice. |
| [RemoveArea](../../aspose.cells/formatconditioncollection/removearea/#removearea)(int, int, int, int) | Rimuovi la formattazione condizionale nell'intervallo. |
| [RemoveCondition](../../aspose.cells/formatconditioncollection/removecondition/)(int) | Rimuove la condizione di formattazione per indice. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionCollectionDemo
    {
        public static void FormatConditionCollectionExample()
        {
            // Crea una nuova Workbook
            Workbook workbook = new Workbook();

            // Ottieni il primo foglio di lavoro
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiunge una formattazione condizionale vuota
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Imposta l'intervallo di formattazione condizionale
            CellArea ca = new CellArea { StartRow = 0, EndRow = 0, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(ca);
            ca = new CellArea { StartRow = 1, EndRow = 1, StartColumn = 1, EndColumn = 1 };
            fcs.AddArea(ca);

            // Aggiunge condizioni
            int conditionIndex1 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");

            // Imposta il colore di sfondo
            FormatCondition fc1 = fcs[conditionIndex1];
            fc1.Style.BackgroundColor = System.Drawing.Color.Red;

            // Salvataggio del file Excel
            workbook.Save("FormatConditionCollectionExample.xlsx");
            workbook.Save("FormatConditionCollectionExample.pdf");
            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


