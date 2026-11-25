---
title: "PivotField.GroupSettings"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotField. Ottiene le impostazioni di raggruppamento del campo pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/groupsettings/
---
## PivotField.GroupSettings property

Ottiene le impostazioni di raggruppamento del campo pivot.

```csharp
public PivotFieldGroupSettings GroupSettings { get; }
```

### Osservazioni

Se questo campo non è raggruppato, verrà restituito Null.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyGroupSettingsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro dal file Excel di origine
            Workbook workbook = new Workbook("example.xlsx");
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi alla prima tabella pivot
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Accedi al secondo campo base (presumendo che esista)
            if (pivotTable.BaseFields.Count > 1)
            {
                PivotField pivotField = pivotTable.BaseFields[1];
                
                // Verifica se il campo ha impostazioni di raggruppamento
                if (pivotField.GroupSettings != null)
                {
                    Console.WriteLine("Field has grouping enabled");
                    Console.WriteLine("Group type: " + pivotField.GroupSettings.Type);
                }
                else
                {
                    Console.WriteLine("Field has no grouping settings");
                }
                
                // Esempio di raggruppamento di un campo numerico
                if (pivotField.GroupSettings == null && 
                    pivotField.PivotItems.Count > 0 && 
                    pivotField.PivotItems[0].Value is double)
                {
                    // Raggruppa per intervallo numerico (intervalli di 10 unità)
                    pivotField.GroupBy(10.0, false);
                    Console.WriteLine("Field grouped by numeric range");
                }
            }
            
            // Salva la cartella di lavoro modificata
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotFieldGroupSettings](../../pivotfieldgroupsettings/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


