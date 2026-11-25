---
title: "WorksheetCollection.TableStyles"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorksheetCollection. Ottiene l'oggetto TableStyles"
type: docs
url: /it/net/aspose.cells/worksheetcollection/tablestyles/
---
## WorksheetCollection.TableStyles property

Ottiene l'oggetto `TableStyles`.

```csharp
public TableStyleCollection TableStyles { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyTableStylesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi alcuni fogli di lavoro
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            
            // Crea e aggiungi stili di tabella
            int styleIndex1 = workbook.Worksheets.TableStyles.AddTableStyle("Style1");
            TableStyle style1 = workbook.Worksheets.TableStyles[styleIndex1];
            
            int styleIndex2 = workbook.Worksheets.TableStyles.AddTableStyle("Style2");
            TableStyle style2 = workbook.Worksheets.TableStyles[styleIndex2];
            
            // Visualizza il conteggio degli stili di tabella
            Console.WriteLine("Table styles count: " + workbook.Worksheets.TableStyles.Count);
            
            // Rimuovi uno stile
            workbook.Worksheets.TableStyles.RemoveAt(0);
            
            // Visualizza il conteggio aggiornato
            Console.WriteLine("Table styles count after removal: " + workbook.Worksheets.TableStyles.Count);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [TableStyleCollection](../../../aspose.cells.tables/tablestylecollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


