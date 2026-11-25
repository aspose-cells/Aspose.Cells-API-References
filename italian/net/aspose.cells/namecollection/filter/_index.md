---
title: "NameCollection.Filter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo NameCollection. Ottiene tutti i nomi definiti per ambito"
type: docs
url: /it/net/aspose.cells/namecollection/filter/
---
## NameCollection.Filter method

Ottiene tutti i nomi definiti per ambito.

```csharp
public Name[] Filter(NameScopeType type, int sheetIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | NameScopeType | Il tipo di ambito. |
| sheetIndex | Int32 | L'indice del foglio. Ha effetto solo quando il tipo di ambito è Worksheet |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodFilterWithNameScopeTypeInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi alcuni nomi alla cartella di lavoro e ai fogli di lavoro
            workbook.Worksheets.Names.Add("GlobalName");
            Worksheet worksheet1 = workbook.Worksheets[0];
            workbook.Worksheets.Names.Add("Sheet1Name");
            Worksheet worksheet2 = workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Names.Add("Sheet2Name");

            // Filtra i nomi per tipo di ambito e indice del foglio
            Name[] workbookScopeNames = workbook.Worksheets.Names.Filter(NameScopeType.Workbook, -1);
            Name[] worksheetScopeNames = workbook.Worksheets.Names.Filter(NameScopeType.Worksheet, -1);
            Name[] sheet1Names = workbook.Worksheets.Names.Filter(NameScopeType.Worksheet, 0);

            // Restituisci i risultati
            Console.WriteLine($"Workbook-scoped names count: {workbookScopeNames.Length}");
            Console.WriteLine($"Worksheet-scoped names count: {worksheetScopeNames.Length}");
            Console.WriteLine($"Sheet1 names count: {sheet1Names.Length}");
        }
    }
}
```

### Vedi anche

* class [Name](../../name/)
* enum [NameScopeType](../../namescopetype/)
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


