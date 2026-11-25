---
title: "WorksheetCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "WorksheetCollection proprietà. Restituisce l'elemento Worksheet all'indice specificato"
type: docs
url: /it/net/aspose.cells/worksheetcollection/item/
---
## WorksheetCollection indexer (1 of 2)

Restituisce l'elemento [`Worksheet`](../../worksheet/) all'indice specificato.

```csharp
public Worksheet this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice a base zero dell'elemento. |

### Valore di ritorno

L'elemento all'indice specificato.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Utilizzo della proprietà Item per accedere alla cella
            Cell cell = cells[0, 0];
            cell.Formula = "=SUM(1, 2, 3)";
            
            workbook.CalculateFormula();
            Console.WriteLine("Cell value: " + cell.IntValue);
        }
    }
}
```

### Vedi anche

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## WorksheetCollection indexer (2 of 2)

Restituisce l'elemento [`Worksheet`](../../worksheet/) con il nome specificato.

```csharp
public Worksheet this[string sheetName] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| sheetName | Nome foglio di lavoro |

### Valore di ritorno

L'elemento con il nome specificato.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi ai fogli di lavoro utilizzando la proprietà Item per indice e nome
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Name = "FirstSheet";
            
            Worksheet sheet2 = workbook.Worksheets.Add("SecondSheet");
            
            // Accedi al foglio di lavoro per nome utilizzando la proprietà Item
            Worksheet accessedSheet = workbook.Worksheets["FirstSheet"];
            
            // Aggiungi dati per dimostrare l'accesso al foglio di lavoro
            Cells cells = accessedSheet.Cells;
            cells["A1"].PutValue("Worksheet accessed successfully!");
            cells["A2"].PutValue(DateTime.Now.ToString());
            
            // Inserisci una colonna nel secondo foglio
            workbook.Worksheets["SecondSheet"].Cells.InsertColumn(1);
            
            // Salva la cartella di lavoro
            workbook.Save("WorksheetCollectionItemDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


