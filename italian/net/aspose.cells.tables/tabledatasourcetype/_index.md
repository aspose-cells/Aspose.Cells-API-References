---
title: "Enum TableDataSourceType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Tables.TableDataSourceType. Rappresenta il tipo di origine dati della tabella"
type: docs
url: /it/net/aspose.cells.tables/tabledatasourcetype/
---
## TableDataSourceType enumeration

Rappresenta il tipo di origine dati della tabella.

```csharp
public enum TableDataSourceType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Worksheet | `0` | Tabella del foglio di lavoro Excel |
| SharePoint | `1` | Elenco collegato a SharePoint in lettura-scrittura |
| XML | `2` | Tabella del mapper XML |
| QueryTable | `3` | Tabella di query |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableDataSourceTypeDemo
    {
        public static void TableDataSourceTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);

            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["B2"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue("Charlie");

            // Aggiungi un ListObject (tabella) al foglio di lavoro
            int listObjectIndex = worksheet.ListObjects.Add(1, 0, 4, 1, true);
            ListObject listObject = worksheet.ListObjects[listObjectIndex];

            // Imposta il nome visualizzato della tabella
            listObject.DisplayName = "SampleTable";

            // Imposta il tipo di origine dati della tabella
            TableDataSourceType dataSourceType = listObject.DataSourceType;

            // Restituisci il tipo di origine dati
            Console.WriteLine("Data Source Type: " + dataSourceType);

            // Salva la cartella di lavoro
            workbook.Save("TableDataSourceTypeExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


