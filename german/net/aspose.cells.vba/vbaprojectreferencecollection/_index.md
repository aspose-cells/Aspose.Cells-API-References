---
title: "Klasse VbaProjectReferenceCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Vba.VbaProjectReferenceCollection Klasse. Stellt alle Verweise des VBA-Projekts dar"
type: docs
url: /de/net/aspose.cells.vba/vbaprojectreferencecollection/
---
## VbaProjectReferenceCollection class

Stellt alle Referenzen des VBA‑Projekts dar.

```csharp
public class VbaProjectReferenceCollection : CollectionBase<VbaProjectReference>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.vba/vbaprojectreferencecollection/item/) { get; } | Erhalte den Verweis in der Liste nach dem Index. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AddControlReferernce](../../aspose.cells.vba/vbaprojectreferencecollection/addcontrolreferernce/)(string, string, string, string) | Füge einen Verweis zu einer manipulierten Typbibliothek und ihrer erweiterten Typbibliothek hinzu. |
| [AddControlRefrernce](../../aspose.cells.vba/vbaprojectreferencecollection/addcontrolrefrernce/)(string, string, string, string) | (**Obsolete.**) Füge einen Verweis zu einer manipulierten Typbibliothek und ihrer erweiterten Typbibliothek hinzu. |
| [AddProjectReferernce](../../aspose.cells.vba/vbaprojectreferencecollection/addprojectreferernce/)(string, string, string) | Fügt einen Verweis zu einem externen VBA-Projekt hinzu. |
| [AddProjectRefrernce](../../aspose.cells.vba/vbaprojectreferencecollection/addprojectrefrernce/)(string, string, string) | (**Obsolete.**) Fügt einen Verweis zu einem externen VBA-Projekt hinzu. |
| [AddRegisteredReference](../../aspose.cells.vba/vbaprojectreferencecollection/addregisteredreference/)(string, string) | Füge einen Verweis zu einer Automation-Typbibliothek hinzu. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(VbaProjectReference) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(VbaProjectReference, IComparer&lt;VbaProjectReference&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, VbaProjectReference, IComparer&lt;VbaProjectReference&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(VbaProjectReference) |  |
| [Copy](../../aspose.cells.vba/vbaprojectreferencecollection/copy/)(VbaProjectReferenceCollection) | Kopiert Verweise aus einem anderen VBA-Projekt. |
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

### Beispiele

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
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();
            
            // VBA-Projekt initialisieren
            VbaProject vbaProject = workbook.VbaProject;
            
            // VBA-Projektreferenz hinzufügen
            vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
            
            // Füge einen weiteren VBA-Projektverweis hinzu
            vbaProject.References.AddControlRefrernce("MSForms", "*\\G{0D452EE1-E08F-101A-852E-02608C4D0BB4}#2.0#0#C:\\Windows\\system32\\FM20.DLL#Microsoft Forms 2.0 Object Library", "twiddledLibid", "extendedLibid");
            
            // Projektverweis hinzufügen
            vbaProject.References.AddProjectRefrernce("MyProject", "absoluteLibid", "relativeLibid");
            
            // Zugriff auf die Verweissammlung
            VbaProjectReferenceCollection references = vbaProject.References;
            
            // Anzeige der Anzahl der Verweise
            Console.WriteLine("Total References: " + references.Count);
            
            // Zugriff auf einen bestimmten Verweis
            VbaProjectReference reference = references[0];
            Console.WriteLine("First Reference Name: " + reference.Name);
            
            // Kopieren von Verweisen aus einer anderen Sammlung (angenommen, anotherVbaProjectReferences ist eine andere VbaProjectReferenceCollection)
            // VbaProjectReferenceCollection anotherVbaProjectReferences = ...;
            // references.Copy(anotherVbaProjectReferences);
            
            // Die Excel-Datei speichern
            workbook.Save("VbaProjectReferenceCollectionExample.xlsm");
        }
    }
}
```

### Siehe auch

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [VbaProjectReference](../vbaprojectreference/)
* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


