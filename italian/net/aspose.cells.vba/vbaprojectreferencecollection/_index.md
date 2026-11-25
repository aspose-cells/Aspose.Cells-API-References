---
title: "Classe VbaProjectReferenceCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Vba.VbaProjectReferenceCollection. Rappresenta tutti i riferimenti del progetto VBA"
type: docs
url: /it/net/aspose.cells.vba/vbaprojectreferencecollection/
---
## VbaProjectReferenceCollection class

Rappresenta tutti i riferimenti del progetto VBA.

```csharp
public class VbaProjectReferenceCollection : CollectionBase<VbaProjectReference>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.vba/vbaprojectreferencecollection/item/) { get; } | Ottieni il riferimento nella lista per indice. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AddControlReferernce](../../aspose.cells.vba/vbaprojectreferencecollection/addcontrolreferernce/)(string, string, string, string) | Aggiungi un riferimento a una libreria di tipo modificata e alla sua libreria di tipo estesa. |
| [AddControlRefrernce](../../aspose.cells.vba/vbaprojectreferencecollection/addcontrolrefrernce/)(string, string, string, string) | (**Obsolete.**) Aggiungi un riferimento a una libreria di tipo modificata e alla sua libreria di tipo estesa. |
| [AddProjectReferernce](../../aspose.cells.vba/vbaprojectreferencecollection/addprojectreferernce/)(string, string, string) | Aggiunge un riferimento a un progetto VBA esterno. |
| [AddProjectRefrernce](../../aspose.cells.vba/vbaprojectreferencecollection/addprojectrefrernce/)(string, string, string) | (**Obsolete.**) Aggiunge un riferimento a un progetto VBA esterno. |
| [AddRegisteredReference](../../aspose.cells.vba/vbaprojectreferencecollection/addregisteredreference/)(string, string) | Aggiungi un riferimento a una libreria di tipo Automation. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(VbaProjectReference) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(VbaProjectReference, IComparer&lt;VbaProjectReference&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, VbaProjectReference, IComparer&lt;VbaProjectReference&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(VbaProjectReference) |  |
| [Copy](../../aspose.cells.vba/vbaprojectreferencecollection/copy/)(VbaProjectReferenceCollection) | Copia i riferimenti da un altro progetto VBA. |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(VbaProjectReference[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(VbaProjectReference[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, VbaProjectReference[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;VbaProjectReference&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;VbaProjectReference&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;VbaProjectReference&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;VbaProjectReference&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;VbaProjectReference&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;VbaProjectReference&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;VbaProjectReference&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;VbaProjectReference&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;VbaProjectReference&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;VbaProjectReference&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(VbaProjectReference) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(VbaProjectReference, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(VbaProjectReference, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(VbaProjectReference) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(VbaProjectReference, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(VbaProjectReference, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaProjectReferenceCollectionDemo
    {
        public static void VbaProjectReferenceCollectionExample()
        {
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();
            
            // Inizializza progetto VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // Aggiungi riferimento al progetto VBA
            vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
            
            // Aggiungi un altro riferimento a progetto VBA
            vbaProject.References.AddControlRefrernce("MSForms", "*\\G{0D452EE1-E08F-101A-852E-02608C4D0BB4}#2.0#0#C:\\Windows\\system32\\FM20.DLL#Microsoft Forms 2.0 Object Library", "twiddledLibid", "extendedLibid");
            
            // Aggiungi riferimento al progetto
            vbaProject.References.AddProjectRefrernce("MyProject", "absoluteLibid", "relativeLibid");
            
            // Accesso alla collezione di riferimenti
            VbaProjectReferenceCollection references = vbaProject.References;
            
            // Visualizzazione del conteggio dei riferimenti
            Console.WriteLine("Total References: " + references.Count);
            
            // Accesso a un riferimento specifico
            VbaProjectReference reference = references[0];
            Console.WriteLine("First Reference Name: " + reference.Name);
            
            // Copia dei riferimenti da un'altra collezione (supponendo che anotherVbaProjectReferences sia un'altra VbaProjectReferenceCollection)
            // VbaProjectReferenceCollection anotherVbaProjectReferences = ...;
            // references.Copy(anotherVbaProjectReferences);
            
            // Salvataggio del file Excel
            workbook.Save("VbaProjectReferenceCollectionExample.xlsm");
        }
    }
}
```

### Vedi anche

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [VbaProjectReference](../vbaprojectreference/)
* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


