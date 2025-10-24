##Class VbaModuleCollection
Aspose.Cells.Vba.VbaModuleCollection class. Represents the list of VbaModule
## VbaModuleCollection class
Represents the list of [`VbaModule`](../vbamodule/)
```csharp
public class VbaModuleCollection : CollectionBase<VbaModule>
```
## Properties
| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.vba/vbamodulecollection/item/) { get; } | Gets [`VbaModule`](../vbamodule/) in the list by the index. (2 indexers) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
## Methods
| Name | Description |
| --- | --- |
| [Add](../../aspose.cells.vba/vbamodulecollection/add/#add_1)(Worksheet) | Adds module for a worksheet. |
| [Add](../../aspose.cells.vba/vbamodulecollection/add/#add)(VbaModuleType, string) | Adds module. |
| [AddDesignerStorage](../../aspose.cells.vba/vbamodulecollection/adddesignerstorage/)(string, byte[]) |  |
| [AddUserForm](../../aspose.cells.vba/vbamodulecollection/adduserform/)(string, string, byte[]) | Inser user form into VBA Project. |
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
| [GetDesignerStorage](../../aspose.cells.vba/vbamodulecollection/getdesignerstorage/)(string) | Represents the data of Designer. |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(VbaModule) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(VbaModule, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(VbaModule, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(VbaModule) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(VbaModule, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(VbaModule, int, int) |  |
| [Remove](../../aspose.cells.vba/vbamodulecollection/remove/#remove_1)(string) | Remove the module by the name |
| [Remove](../../aspose.cells.vba/vbamodulecollection/remove/#remove)(Worksheet) | Removes module for a worksheet. |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
### Examples
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
// Create a new workbook
Workbook workbook = new Workbook();
// Access the VBA project
VbaProject vbaProject = workbook.VbaProject;
// Add a new class module
int index = vbaProject.Modules.Add(VbaModuleType.Class, "TestClass");
// Get the added module and add some code
VbaModule module = vbaProject.Modules[index];
module.Codes = "Public Sub TestMethod()\r\n    MsgBox \"Hello from VBA!\"\r\nEnd Sub";
// Save as macro-enabled workbook
workbook.Save("VbaModuleCollectionDemo.xlsm", SaveFormat.Xlsm);
}
}
}
```
### See Also
* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [VbaModule](../vbamodule/)
* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)
