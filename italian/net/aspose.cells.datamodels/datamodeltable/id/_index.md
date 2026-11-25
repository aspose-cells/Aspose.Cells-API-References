---
title: "DataModelTable.Id"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataModelTable. Ottiene l'id della tabella del modello di dati"
type: docs
url: /it/net/aspose.cells.datamodels/datamodeltable/id/
---
## DataModelTable.Id property

Ottiene l'ID della tabella del modello di dati.

```csharp
public string Id { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using Aspose.Cells.Tables;
    using System;

    public class DataModelTablePropertyIdDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per creare una tabella
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Item 2");

            // Crea un ListObject (tabella)
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];

            // Ottieni il DataModelTable (è di sola lettura nella cartella di lavoro)
            DataModelTable dataModelTable = workbook.DataModel.Tables[0];

            // Visualizza il valore corrente dell'Id
            Console.WriteLine("Current DataModelTable Id: " + dataModelTable.Id);

            // Nota: la proprietà Id è di sola lettura, quindi non possiamo impostarla
            // Questo dimostra come accedere e utilizzare l'Id esistente

            // Esempio di utilizzo: confronta gli ID delle tabelle quando lavori con più tabelle
            DataModelTable secondTable = null;
            if (workbook.DataModel.Tables.Count > 1)
            {
                secondTable = workbook.DataModel.Tables[1];
                if (dataModelTable.Id != secondTable.Id)
                {
                    Console.WriteLine("Different table IDs detected");
                }
            }

            // Salva la cartella di lavoro
            workbook.Save("DataModelTableIdDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [DataModelTable](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


