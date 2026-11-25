---
title: "CommentCollection.RemoveAt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CommentCollection. Rimuove il commento della cella specifica"
type: docs
url: /it/net/aspose.cells/commentcollection/removeat/
---
## RemoveAt(string) {#removeat_2}

Rimuove il commento della cella specifica.

```csharp
public void RemoveAt(string cellName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellName | String | Il nome della cella che contiene un commento. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionMethodRemoveAtWithStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi commenti alle celle usando i nomi delle celle
            int commentIndex1 = worksheet.Comments.Add("A1");
            worksheet.Comments[commentIndex1].Note = "Comment in A1";
            
            int commentIndex2 = worksheet.Comments.Add("B2");
            worksheet.Comments[commentIndex2].Note = "Comment in B2";
            
            int commentIndex3 = worksheet.Comments.Add("C3");
            worksheet.Comments[commentIndex3].Note = "Comment in C3";
            
            // Rimuovi il commento nella cella B2 usando RemoveAt con parametro stringa
            worksheet.Comments.RemoveAt("B2");
            
            // Salva la cartella di lavoro
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveAt(int, int) {#removeat_1}

Rimuove il commento della cella specifica.

```csharp
public void RemoveAt(int row, int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | L'indice della riga. |
| colonna | Int32 | l'indice della colonna. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionMethodRemoveAtWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi commenti alle celle usando i riferimenti di cella
            int comment1Index = worksheet.Comments.Add("A1");
            worksheet.Comments[comment1Index].Note = "First comment";
            
            int comment2Index = worksheet.Comments.Add("B2");
            worksheet.Comments[comment2Index].Note = "Second comment";
            
            int comment3Index = worksheet.Comments.Add("C3");
            worksheet.Comments[comment3Index].Note = "Third comment";
            
            // Rimuovi il commento alla riga 1, colonna 1 (B2)
            worksheet.Comments.RemoveAt(1, 1);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


