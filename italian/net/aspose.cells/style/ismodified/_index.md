---
title: "Style.IsModified"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Style. Verifica se le proprietà specificate dello stile sono state modificate. Utilizzato per lo stile dei ConditionalFormattings per verificare se le proprietà specificate di questo stile devono essere utilizzate durante l'applicazione dei ConditionalFormattings su una cella"
type: docs
url: /it/net/aspose.cells/style/ismodified/
---
## Style.IsModified method

Verifica se le proprietà specificate dello stile sono state modificate. Utilizzato per lo stile dei ConditionalFormattings per verificare se le proprietà specificate di questo stile devono essere utilizzate quando si applicano i ConditionalFormattings su una cella.

```csharp
public bool IsModified(StyleModifyFlag modifyFlag)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| modifyFlag | StyleModifyFlag | Flag di modifica dello stile |

### Valore di ritorno

vero se le proprietà specificate sono state modificate

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodIsModifiedWithStyleModifyFlagDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ottieni lo stile della cella A1
            Style style = worksheet.Cells["A1"].GetStyle();
            
            // Modifica il motivo (sfondo) dello stile
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            
            // Verifica se il motivo è stato modificato
            bool isPatternModified = style.IsModified(StyleModifyFlag.Pattern);
            
            // Restituisci il risultato
            Console.WriteLine("Is pattern modified: " + isPatternModified);
        }
    }
}
```

### Vedi anche

* enum [StyleModifyFlag](../../stylemodifyflag/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


