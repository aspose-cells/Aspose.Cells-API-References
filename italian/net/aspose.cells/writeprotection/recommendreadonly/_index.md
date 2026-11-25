---
title: "WriteProtection.RecommendReadOnly"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WriteProtection. Indica se l'opzione 'Read Only Recommended' è selezionata"
type: docs
url: /it/net/aspose.cells/writeprotection/recommendreadonly/
---
## WriteProtection.RecommendReadOnly property

Indica se l'opzione Consiglia sola lettura è selezionata.

```csharp
public bool RecommendReadOnly { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WriteProtectionPropertyRecommendReadOnlyDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al foglio di lavoro e aggiungi alcuni dati di esempio
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");

            // Imposta RecommendReadOnly su true
            workbook.Settings.WriteProtection.RecommendReadOnly = true;
            
            // Verifica che la proprietà sia impostata
            Console.WriteLine("RecommendReadOnly: " + workbook.Settings.WriteProtection.RecommendReadOnly);
            Console.WriteLine("IsWriteProtected: " + workbook.Settings.WriteProtection.IsWriteProtected);

            // Salva la cartella di lavoro
            workbook.Save("output_recommend_readonly.xlsx");

            // Carica la cartella di lavoro salvata per verificare che le impostazioni persistano
            Workbook loadedWorkbook = new Workbook("output_recommend_readonly.xlsx");
            Console.WriteLine("After loading - RecommendReadOnly: " + loadedWorkbook.Settings.WriteProtection.RecommendReadOnly);
            Console.WriteLine("After loading - IsWriteProtected: " + loadedWorkbook.Settings.WriteProtection.IsWriteProtected);
        }
    }
}
```

### Vedi anche

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


