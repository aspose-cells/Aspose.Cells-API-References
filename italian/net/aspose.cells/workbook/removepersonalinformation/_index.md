---
title: "Workbook.RemovePersonalInformation"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Rimuove le informazioni personali"
type: docs
url: /it/net/aspose.cells/workbook/removepersonalinformation/
---
## Workbook.RemovePersonalInformation method

Rimuove le informazioni personali.

```csharp
public void RemovePersonalInformation()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRemovePersonalInformationDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Aggiungi un commento con le informazioni sull'autore
            int commentIndex = sheet.Comments.Add("A1");
            sheet.Comments[commentIndex].Note = "Sample comment";
            sheet.Comments[commentIndex].Author = "Test Author";
            
            // Visualizza le informazioni sull'autore originale
            Console.WriteLine("Before removal - Comment Author: " + sheet.Comments[commentIndex].Author);
            
            // Rimuovi le informazioni personali
            wb.RemovePersonalInformation();
            
            // Salva la cartella di lavoro
            wb.Save("output.xlsx", SaveFormat.Xlsx);
            
            // Ricarica per verificare la rimozione
            Workbook wb2 = new Workbook("output.xlsx");
            Console.WriteLine("After removal - Comment Author: " + wb2.Worksheets[0].Comments[commentIndex].Author);
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


