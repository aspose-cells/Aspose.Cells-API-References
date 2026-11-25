---
title: "Classe OdsCellFieldCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Ods.OdsCellFieldCollection. Rappresenta i campi di ODS"
type: docs
url: /it/net/aspose.cells.ods/odscellfieldcollection/
---
## OdsCellFieldCollection class

Rappresenta i campi di ODS.

```csharp
public class OdsCellFieldCollection : CollectionBase<OdsCellField>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.ods/odscellfieldcollection/item/) { get; } | Restituisce il campo per indice. (2 indicizzatori) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells.ods/odscellfieldcollection/add/)(int, int, OdsCellFieldType, string) | Aggiunge un campo. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(OdsCellField) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(OdsCellField, IComparer&lt;OdsCellField&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, OdsCellField, IComparer&lt;OdsCellField&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(OdsCellField) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(OdsCellField[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(OdsCellField[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, OdsCellField[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;OdsCellField&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;OdsCellField&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;OdsCellField&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;OdsCellField&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;OdsCellField&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;OdsCellField&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;OdsCellField&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;OdsCellField&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;OdsCellField&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;OdsCellField&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(OdsCellField) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(OdsCellField, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(OdsCellField, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(OdsCellField) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(OdsCellField, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(OdsCellField, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
| [UpdateFieldsValue](../../aspose.cells.ods/odscellfieldcollection/updatefieldsvalue/)() | Aggiorna il valore dei campi nelle celle. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;

    public class OdsCellFieldCollectionDemo
    {
        public static void OdsCellFieldCollectionExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Accedi alla OdsCellFieldCollection
            OdsCellFieldCollection odsCellFields = cells.OdsCellFields;

            // Aggiungi campi alla OdsCellFieldCollection
            int fieldIndex1 = odsCellFields.Add(0, 0, OdsCellFieldType.Date, "yyyy-MM-dd");
            int fieldIndex2 = odsCellFields.Add(1, 1, OdsCellFieldType.SheetName, null);
            int fieldIndex3 = odsCellFields.Add(2, 2, OdsCellFieldType.Title, null);

            // Aggiorna il valore dei campi nelle celle
            odsCellFields.UpdateFieldsValue();

            // Salva la cartella di lavoro
            workbook.Save("OdsCellFieldCollectionExample.ods");

            return;
        }
    }
}
```

### Vedi anche

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [OdsCellField](../odscellfield/)
* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


