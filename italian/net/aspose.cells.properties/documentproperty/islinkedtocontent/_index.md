---
title: "DocumentProperty.IsLinkedToContent"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DocumentProperty. Indica se questa proprietà è collegata al contenuto"
type: docs
url: /it/net/aspose.cells.properties/documentproperty/islinkedtocontent/
---
## DocumentProperty.IsLinkedToContent property

Indica se questa proprietà è collegata al contenuto

```csharp
public bool IsLinkedToContent { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyPropertyIsLinkedToContentDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi dati di esempio alle celle
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Company Name";
            worksheet.Cells["B1"].Value = "Company Address";

            // Crea proprietà documento personalizzate collegate
            workbook.CustomDocumentProperties.AddLinkToContent("Company", "A1");
            workbook.CustomDocumentProperties.AddLinkToContent("Address", "B1");

            // Ottieni e verifica la proprietà IsLinkedToContent
            DocumentProperty companyProp = workbook.CustomDocumentProperties["Company"];
            Console.WriteLine($"Is 'Company' property linked to content: {companyProp.IsLinkedToContent}");
            Console.WriteLine($"Linked source: {companyProp.Source}");
            Console.WriteLine($"Current value: {companyProp.Value}");

            // Aggiorna il valore della cella e aggiorna le proprietà collegate
            worksheet.Cells["A1"].Value = "Updated Company Name";
            workbook.CustomDocumentProperties.UpdateLinkedPropertyValue();

            // Verifica che la proprietà sia stata aggiornata
            Console.WriteLine($"Updated value: {companyProp.Value}");

            // Salva la cartella di lavoro
            workbook.Save("LinkedPropertiesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


