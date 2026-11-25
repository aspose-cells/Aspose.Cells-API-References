---
title: "WorksheetCollection.GetSheetByCodeName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo WorksheetCollection. Ottiene il foglio di lavoro per nome codice"
type: docs
url: /it/net/aspose.cells/worksheetcollection/getsheetbycodename/
---
## WorksheetCollection.GetSheetByCodeName method

Ottiene il foglio di lavoro per nome codice.

```csharp
public Worksheet GetSheetByCodeName(string codeName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| codeName | String | Nome codice del foglio di lavoro. |

### Valore di ritorno

L'elemento con il nome codice specificato.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodGetSheetByCodeNameWithStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi fogli di lavoro e imposta i loro nomi codice
            Worksheet sheet1 = workbook.Worksheets.Add("Sheet1");
            sheet1.CodeName = "MainSheet";
            
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            sheet2.CodeName = "DataSheet";

            // Ottieni il foglio di lavoro per nome codice
            Worksheet mainSheet = workbook.Worksheets.GetSheetByCodeName("MainSheet");
            Worksheet dataSheet = workbook.Worksheets.GetSheetByCodeName("DataSheet");

            // Dimostra l'uso scrivendo nelle celle
            mainSheet.Cells["A1"].PutValue("This is Main Sheet");
            dataSheet.Cells["A1"].PutValue("This is Data Sheet");

            // Salva la cartella di lavoro
            workbook.Save("GetSheetByCodeNameDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


