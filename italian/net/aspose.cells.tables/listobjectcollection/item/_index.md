---
title: "ListObjectCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListObjectCollection. Ottiene il ListObject per indice"
type: docs
url: /it/net/aspose.cells.tables/listobjectcollection/item/
---
## ListObjectCollection indexer (1 of 2)

Ottiene il ListObject per indice.

```csharp
public ListObject this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice. |

### Valore di ritorno

Il ListObject

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            
            // Crea un oggetto elenco
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = worksheet.ListObjects[index];
            
            // Accedi all'oggetto ListObject usando la proprietà Item
            ListObject firstListObject = worksheet.ListObjects[0];
            
            // Imposta lo stile della tabella
            firstListObject.TableStyleType = TableStyleType.TableStyleMedium2;
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [ListObject](../../listobject/)
* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## ListObjectCollection indexer (2 of 2)

Ottiene il ListObject per nome specificato.

```csharp
public ListObject this[string tableName] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| tableName | Nome del ListObject. |

### Valore di ritorno

Il ListObject

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Crea un oggetto elenco
            int index = worksheet.ListObjects.Add("A1", "B3", true);
            ListObject listObj = worksheet.ListObjects[index];
            listObj.DisplayName = "PersonTable";

            // Accedi all'oggetto ListObject usando la proprietà Item per nome
            ListObject retrievedListObj = worksheet.ListObjects["PersonTable"];
            
            // Dimostra l'uso convertendo in un intervallo
            retrievedListObj.ConvertToRange();

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [ListObject](../../listobject/)
* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


