---
title: "Klass VbaProjectReferenceCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Vba.VbaProjectReferenceCollection-klass. Representerar alla referenser till VBA-projektet"
type: docs
url: /sv/net/aspose.cells.vba/vbaprojectreferencecollection/
---
## VbaProjectReferenceCollection class

Representerar alla referenser till VBA‑projektet.

```csharp
public class VbaProjectReferenceCollection : CollectionBase<VbaProjectReference>
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.vba/vbaprojectreferencecollection/item/) { get; } | Hämta referensen i listan efter index. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [AddControlReferernce](../../aspose.cells.vba/vbaprojectreferencecollection/addcontrolreferernce/)(string, string, string, string) | Lägg till en referens till ett vridet typbibliotek och dess utökade typbibliotek. |
| [AddControlRefrernce](../../aspose.cells.vba/vbaprojectreferencecollection/addcontrolrefrernce/)(string, string, string, string) | (**Obsolete.**) Lägg till en referens till ett vridet typbibliotek och dess utökade typbibliotek. |
| [AddProjectReferernce](../../aspose.cells.vba/vbaprojectreferencecollection/addprojectreferernce/)(string, string, string) | Lägger till en referens till ett externt VBA-projekt. |
| [AddProjectRefrernce](../../aspose.cells.vba/vbaprojectreferencecollection/addprojectrefrernce/)(string, string, string) | (**Obsolete.**) Lägger till en referens till ett externt VBA-projekt. |
| [AddRegisteredReference](../../aspose.cells.vba/vbaprojectreferencecollection/addregisteredreference/)(string, string) | Lägg till en referens till ett automations-typbibliotek. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(VbaProjectReference) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(VbaProjectReference, IComparer&lt;VbaProjectReference&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, VbaProjectReference, IComparer&lt;VbaProjectReference&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(VbaProjectReference) |  |
| [Copy](../../aspose.cells.vba/vbaprojectreferencecollection/copy/)(VbaProjectReferenceCollection) | Kopierar referenser från ett annat VBA-projekt. |
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

### Exempel

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
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();
            
            // Initiera VBA-projekt
            VbaProject vbaProject = workbook.VbaProject;
            
            // Lägg till VBA-projektreferens
            vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
            
            // Lägg till en annan VBA-projektreferens
            vbaProject.References.AddControlRefrernce("MSForms", "*\\G{0D452EE1-E08F-101A-852E-02608C4D0BB4}#2.0#0#C:\\Windows\\system32\\FM20.DLL#Microsoft Forms 2.0 Object Library", "twiddledLibid", "extendedLibid");
            
            // Lägg till projektreferens
            vbaProject.References.AddProjectRefrernce("MyProject", "absoluteLibid", "relativeLibid");
            
            // Åtkomst till referenssamlingen
            VbaProjectReferenceCollection references = vbaProject.References;
            
            // Visar antalet referenser
            Console.WriteLine("Total References: " + references.Count);
            
            // Åtkomst till en specifik referens
            VbaProjectReference reference = references[0];
            Console.WriteLine("First Reference Name: " + reference.Name);
            
            // Kopierar referenser från en annan samling (förutsatt att anotherVbaProjectReferences är en annan VbaProjectReferenceCollection)
            // VbaProjectReferenceCollection anotherVbaProjectReferences = ...;
            // references.Copy(anotherVbaProjectReferences);
            
            // Sparar Excel-filen
            workbook.Save("VbaProjectReferenceCollectionExample.xlsm");
        }
    }
}
```

### Se även

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [VbaProjectReference](../vbaprojectreference/)
* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


