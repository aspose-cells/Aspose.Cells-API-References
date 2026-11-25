---
title: "Column.GroupLevel"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Column. Ottiene il livello di raggruppamento della colonna"
type: docs
url: /it/net/aspose.cells/column/grouplevel/
---
## Column.GroupLevel property

Ottiene il livello di gruppo della colonna.

```csharp
public byte GroupLevel { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnPropertyGroupLevelDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Raggruppa colonne (parametro isHidden impostato su false)
            worksheet.Cells.GroupColumns(0, 2, false);
            
            // Ottieni il livello di raggruppamento della prima colonna
            int groupLevel = worksheet.Cells.Columns[0].GroupLevel;
            
            // Stampa il livello di raggruppamento
            Console.WriteLine("Group level of first column: " + groupLevel);
            
            // Salva la cartella di lavoro
            workbook.Save("GroupLevelDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


