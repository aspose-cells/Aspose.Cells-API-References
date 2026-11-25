---
title: "Classe VbaModuleCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Vba.VbaModuleCollection. Rappresenta l'elenco di VbaModule"
type: docs
url: /it/net/aspose.cells.vba/vbamodulecollection/
---
## VbaModuleCollection class

Rappresenta l'elenco di [`VbaModule`](../vbamodule/)

```csharp
public class VbaModuleCollection : CollectionBase<VbaModule>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.vba/vbamodulecollection/item/) { get; } | Ottiene [`VbaModule`](../vbamodule/) nell'elenco per indice. (2 indicizzatori) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells.vba/vbamodulecollection/add/#add_1)(Worksheet) | Aggiunge un modulo per un foglio di lavoro. |
| [Add](../../aspose.cells.vba/vbamodulecollection/add/#add)(VbaModuleType, string) | Aggiunge un modulo. |
| [AddDesignerStorage](../../aspose.cells.vba/vbamodulecollection/adddesignerstorage/)(string, byte[]) |  |
| [AddUserForm](../../aspose.cells.vba/vbamodulecollection/adduserform/)(string, string, byte[]) | Inserisci il modulo utente nel progetto VBA. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(VbaModule) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(VbaModule, IComparer&lt;VbaModule&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, VbaModule, IComparer&lt;VbaModule&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(VbaModule) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(VbaModule[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(VbaModule[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, VbaModule[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;VbaModule&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;VbaModule&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;VbaModule&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;VbaModule&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;VbaModule&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;VbaModule&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;VbaModule&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;VbaModule&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;VbaModule&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;VbaModule&gt;) |  |
| [GetDesignerStorage](../../aspose.cells.vba/vbamodulecollection/getdesignerstorage/)(string) | Rappresenta i dati del Designer. |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(VbaModule) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(VbaModule, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(VbaModule, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(VbaModule) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(VbaModule, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(VbaModule, int, int) |  |
| [Remove](../../aspose.cells.vba/vbamodulecollection/remove/#remove_1)(string) | Rimuovi il modulo per nome |
| [Remove](../../aspose.cells.vba/vbamodulecollection/remove/#remove)(Worksheet) | Rimuove il modulo per un foglio di lavoro. |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaClassVbaModuleCollectionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al progetto VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // Aggiungi un nuovo modulo di classe
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "TestClass");
            
            // Ottieni il modulo aggiunto e aggiungi del codice
            VbaModule module = vbaProject.Modules[index];
            module.Codes = "Public Sub TestMethod()\r\n    MsgBox \"Hello from VBA!\"\r\nEnd Sub";
            
            // Salva come cartella di lavoro con macro abilitata
            workbook.Save("VbaModuleCollectionDemo.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Vedi anche

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [VbaModule](../vbamodule/)
* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


