---
title: "Classe DataModel"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.DataModels.DataModel. Rappresenta il modello dati"
type: docs
url: /it/net/aspose.cells.datamodels/datamodel/
---
## DataModel class

Rappresenta il modello di dati.

```csharp
public class DataModel
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Relationships](../../aspose.cells.datamodels/datamodel/relationships/) { get; } | Ottiene tutte le relazioni delle tabelle nel modello dati. |
| [Tables](../../aspose.cells.datamodels/datamodel/tables/) { get; } | Ottiene tutte le tabelle nel modello dati. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelsClassDataModelDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ottieni il DataModel dalla cartella di lavoro invece di creare una nuova istanza
            DataModel dataModel = workbook.DataModel;

            // Dimostra l'accesso a tabelle e relazioni (proprietà di sola lettura)
            Console.WriteLine("Number of tables in DataModel: " + dataModel.Tables.Count);
            Console.WriteLine("Number of relationships in DataModel: " + dataModel.Relationships.Count);

            // Nota: Poiché le tabelle e le relazioni sono collezioni di sola lettura,
            // possiamo solo accedere agli elementi esistenti ma non modificarli direttamente

            // Salva la cartella di lavoro (DataModel è tipicamente usato internamente da Aspose.Cells)
            workbook.Save("DataModelDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.DataModels](../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../)


