---
title: "WorksheetCollection.RemoveAt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo WorksheetCollection. Rimuove l'elemento con un nome specificato"
type: docs
url: /it/net/aspose.cells/worksheetcollection/removeat/
---
## RemoveAt(string) {#removeat_2}

Rimuove l'elemento a un nome specificato.

```csharp
public void RemoveAt(string name)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome dell'elemento da rimuovere. |

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRemoveAtWithStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook wb = new Workbook();
            
            // Aggiungi alcuni fogli di lavoro
            wb.Worksheets.Add("Sheet2");
            wb.Worksheets.Add("Sheet3");
            
            // Aggiungi un intervallo denominato (fisso)
            int nameIndex = wb.Worksheets.Names.Add("testname");
            wb.Worksheets.Names[nameIndex].RefersTo = "=[Book1.xlsx]Sheet1!$A1";
            
            // Dimostra RemoveAt con parametro stringa
            Console.WriteLine($"Before removal - Worksheet count: {wb.Worksheets.Count}");
            wb.Worksheets.RemoveAt("Sheet1");
            Console.WriteLine($"After removal - Worksheet count: {wb.Worksheets.Count}");
            
            // Salva la cartella di lavoro
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Xlsx);
            }
        }
    }
}
```

### Vedi anche

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveAt(int) {#removeat}

Rimuove l'elemento a un indice specificato.

```csharp
public void RemoveAt(int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | Il valore dell'indice dell'elemento da rimuovere. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook wb = new Workbook();
            
            // Aggiungi alcuni fogli di lavoro
            wb.Worksheets.Add("Sheet1");
            wb.Worksheets.Add("Sheet2");
            wb.Worksheets.Add("Sheet3");

            // Visualizza il conteggio originale dei fogli di lavoro
            Console.WriteLine($"Original worksheet count: {wb.Worksheets.Count}");

            // Rimuovi il foglio di lavoro all'indice 1 (secondo foglio di lavoro)
            wb.Worksheets.RemoveAt(1);

            // Visualizza il conteggio aggiornato dei fogli di lavoro
            Console.WriteLine($"After removal, worksheet count: {wb.Worksheets.Count}");

            // Salva la cartella di lavoro
            wb.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


