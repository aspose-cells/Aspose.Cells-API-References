---
title: "Klass VbaModuleCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Vba.VbaModuleCollection-klass. Representerar listan av VbaModule"
type: docs
url: /sv/net/aspose.cells.vba/vbamodulecollection/
---
## VbaModuleCollection class

Representerar listan av [`VbaModule`](../vbamodule/)

```csharp
public class VbaModuleCollection : CollectionBase<VbaModule>
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.vba/vbamodulecollection/item/) { get; } | Hämtar [`VbaModule`](../vbamodule/) i listan efter index. (2 indexerare) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells.vba/vbamodulecollection/add/#add_1)(Worksheet) | Lägger till modul för ett kalkylblad. |
| [Add](../../aspose.cells.vba/vbamodulecollection/add/#add)(VbaModuleType, string) | Lägger till modul. |
| [AddDesignerStorage](../../aspose.cells.vba/vbamodulecollection/adddesignerstorage/)(string, byte[]) |  |
| [AddUserForm](../../aspose.cells.vba/vbamodulecollection/adduserform/)(string, string, byte[]) | Infoga användarformulär i VBA-projektet. |
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
| [GetDesignerStorage](../../aspose.cells.vba/vbamodulecollection/getdesignerstorage/)(string) | Representerar data för Designer. |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(VbaModule) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(VbaModule, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(VbaModule, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(VbaModule) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(VbaModule, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(VbaModule, int, int) |  |
| [Remove](../../aspose.cells.vba/vbamodulecollection/remove/#remove_1)(string) | Ta bort modulen efter namn |
| [Remove](../../aspose.cells.vba/vbamodulecollection/remove/#remove)(Worksheet) | Tar bort modul för ett kalkylblad. |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till VBA-projektet
            VbaProject vbaProject = workbook.VbaProject;
            
            // Lägg till en ny klassmodul
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "TestClass");
            
            // Hämta den tillagda modulen och lägg till lite kod
            VbaModule module = vbaProject.Modules[index];
            module.Codes = "Public Sub TestMethod()\r\n    MsgBox \"Hello from VBA!\"\r\nEnd Sub";
            
            // Spara som makroaktiverad arbetsbok
            workbook.Save("VbaModuleCollectionDemo.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Se även

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [VbaModule](../vbamodule/)
* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


