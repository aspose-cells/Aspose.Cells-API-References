---
title: "FormatConditionCollection.RemoveArea"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FormatConditionCollection. Rimuove l'intervallo di celle formattate condizionalmente per indice"
type: docs
url: /it/net/aspose.cells/formatconditioncollection/removearea/
---
## RemoveArea(int) {#removearea_1}

Rimuove l'intervallo di celle formattato condizionalmente per indice.

```csharp
public void RemoveArea(int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | L'indice dell'intervallo di celle formattate condizionalmente da rimuovere. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodRemoveAreaWithInt32Demo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi formattazione condizionale
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection formatConditionCollection = conditionalFormattings[index];

            // Aggiungere aree da formattare
            formatConditionCollection.AddArea(CellArea.CreateCellArea(0, 0, 10, 5)); // First area
            formatConditionCollection.AddArea(CellArea.CreateCellArea(5, 5, 15, 10)); // Second area

            // Aggiungere una condizione
            formatConditionCollection.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");

            // Visualizzare il conteggio iniziale delle aree (sappiamo di aver aggiunto 2 aree)
            Console.WriteLine("Areas before removal: 2");

            // Rimuovere la seconda area (indice 1)
            formatConditionCollection.RemoveArea(1);

            // Visualizzare il conteggio delle aree dopo la rimozione (sappiamo di aver rimosso 1 area)
            Console.WriteLine("Areas after removal: 1");

            // Salva la cartella di lavoro
            workbook.Save("RemoveAreaDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveArea(int, int, int, int) {#removearea}

Rimuovi la formattazione condizionale nell'intervallo.

```csharp
public bool RemoveArea(int startRow, int startColumn, int totalRows, int totalColumns)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | Int32 | La startRow dell'intervallo. |
| startColumn | Int32 | La startColumn dell'intervallo. |
| totalRows | Int32 | Il numero di righe dell'intervallo. |
| totalColumns | Int32 | Il numero di colonne dell'intervallo. |

### Valore di ritorno

Restituisce TRUE, questa FormatCondtionCollection dovrebbe essere rimossa.

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodRemoveAreaWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            
            int idx = cfc.Add();
            FormatConditionCollection fcc = cfc[idx];
            
            // Aggiungere area iniziale
            CellArea initialArea = CellArea.CreateCellArea(0, 0, 0, 0);
            fcc.AddArea(initialArea);
            
            // Aggiungi condizione
            idx = fcc.AddCondition(FormatConditionType.Expression);
            FormatCondition fc = fcc[idx];
            fc.Formula1 = "=A1>0";
            fc.Style.Font.Color = Color.Red;
            
            // Dimostrare RemoveArea con parametri Int32
            Console.WriteLine("Before removal - Areas count: " + fcc.Count);
            fcc.RemoveArea(0, 0, 1, 1); // Remove the initial area
            Console.WriteLine("After removal - Areas count: " + fcc.Count);
            
            // Aggiungi nuova area
            CellArea newArea = CellArea.CreateCellArea(1, 1, 1, 1);
            fcc.AddArea(newArea);
            Console.WriteLine("After adding new area - Areas count: " + fcc.Count);
        }
    }
}
```

### Vedi anche

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


