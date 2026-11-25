---
title: "Class DeleteBlankOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.DeleteBlankOptions class. Rappresenta l'impostazione per eliminare celle/righe/colonne vuote"
type: docs
url: /it/net/aspose.cells/deleteblankoptions/
---
## DeleteBlankOptions class

Rappresenta l'impostazione per l'eliminazione di celle/righe/colonne vuote.

```csharp
public class DeleteBlankOptions : DeleteOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [DeleteBlankOptions](deleteblankoptions/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DrawingsAsBlank](../../aspose.cells/deleteblankoptions/drawingsasblank/) { get; set; } | Indica se gli oggetti correlati al disegno, come immagine, forma, grafico... saranno considerati vuoti. Il valore predefinito è true. |
| [EmptyFormulaValueAsBlank](../../aspose.cells/deleteblankoptions/emptyformulavalueasblank/) { get; set; } | Se una cella verrà considerata vuota quando è una formula e il risultato calcolato è null o stringa vuota. Il valore predefinito è false. |
| [EmptyStringAsBlank](../../aspose.cells/deleteblankoptions/emptystringasblank/) { get; set; } | Indica se una cella verrà considerata vuota quando il suo valore è una stringa vuota. Il valore predefinito è true. |
| [EndIndex](../../aspose.cells/deleteblankoptions/endindex/) { get; set; } | Specifica l'indice di riga/colonna finale (inclusivo) dell'intervallo da controllare e cancellare righe/colonne vuote. Il valore predefinito è -1 e -1 indica l'intervallo massimo di tutti gli oggetti (celle, disegni, ...) che devono essere controllati. |
| [FormulaChangeMonitor](../../aspose.cells/deleteoptions/formulachangemonitor/) { get; set; } | Ottiene/imposta il monitor per tracciare le modifiche causate dall'eliminazione. (Ereditato da [`DeleteOptions`](../deleteoptions/).) |
| [MergedCellsShrinkType](../../aspose.cells/deleteblankoptions/mergedcellsshrinktype/) { get; set; } | Indica come elaborare le celle unite quando si eliminano righe/colonne vuote. |
| [StartIndex](../../aspose.cells/deleteblankoptions/startindex/) { get; set; } | Specifica l'indice di riga/colonna iniziale dell'intervallo da controllare e cancellare righe/colonne vuote. |
| [UpdateReference](../../aspose.cells/deleteoptions/updatereference/) { get; set; } | Indica se aggiornare i riferimenti in altri fogli di lavoro. (Ereditato da [`DeleteOptions`](../deleteoptions/).) |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DeleteBlankOptionsDemo
    {
        public static void DeleteBlankOptionsExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola il foglio di lavoro con alcuni dati
            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue("");
            worksheet.Cells["A3"].PutValue("More Data");
            worksheet.Cells["A4"].PutValue("");
            worksheet.Cells["A5"].PutValue("Even More Data");

            // Crea un'istanza di DeleteBlankOptions
            DeleteBlankOptions options = new DeleteBlankOptions
            {
                EmptyStringAsBlank = true,
                EmptyFormulaValueAsBlank = false,
                UpdateReference = true
            };

            // Elimina le righe vuote in base alle opzioni
            worksheet.Cells.DeleteBlankRows(options);

            // Salva la cartella di lavoro
            workbook.Save("DeleteBlankOptionsExample.xlsx");
            workbook.Save("DeleteBlankOptionsExample.pdf");
            return;
        }
    }
}
```

### Vedi anche

* class [DeleteOptions](../deleteoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


