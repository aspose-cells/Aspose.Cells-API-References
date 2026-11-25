---
title: "CustomDocumentPropertyCollection.UpdateLinkedPropertyValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CustomDocumentPropertyCollection. Aggiorna i valori di tutte le proprietà personalizzate collegate al contenuto, utilizza il valore della cella dell'intervallo collegato per aggiornare il valore della proprietà personalizzata"
type: docs
url: /it/net/aspose.cells.properties/customdocumentpropertycollection/updatelinkedpropertyvalue/
---
## CustomDocumentPropertyCollection.UpdateLinkedPropertyValue method

Aggiorna i valori di tutte le proprietà personalizzate collegate al contenuto(use il valore della cella dell'intervallo collegato per aggiornare il valore della proprietà personalizzata).

```csharp
public void UpdateLinkedPropertyValue()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodUpdateLinkedPropertyValueDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi alcuni dati alle celle che saranno collegate alle proprietà personalizzate
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "InitialValue1";
            worksheet.Cells["B1"].Value = "InitialValue2";

            // Aggiungi proprietà personalizzate collegate
            workbook.CustomDocumentProperties.AddLinkToContent("CompanyName", "A1");
            workbook.CustomDocumentProperties.AddLinkToContent("Department", "B1");

            // Aggiorna i valori delle celle
            worksheet.Cells["A1"].Value = "UpdatedValue1";
            worksheet.Cells["B1"].Value = "UpdatedValue2";

            // Aggiorna i valori delle proprietà collegate
            workbook.CustomDocumentProperties.UpdateLinkedPropertyValue();

            // Visualizza i valori delle proprietà aggiornate
            Console.WriteLine("CompanyName: " + workbook.CustomDocumentProperties["CompanyName"].Value);
            Console.WriteLine("Department: " + workbook.CustomDocumentProperties["Department"].Value);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


