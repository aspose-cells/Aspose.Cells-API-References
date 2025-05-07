---
title: VbaProject.Modules
second_title: Aspose.Cells for .NET API Reference
description: VbaProject property. Gets all VbaModule objects
type: docs
url: /net/aspose.cells.vba/vbaproject/modules/
---
## VbaProject.Modules property

Gets all [`VbaModule`](../../vbamodule/) objects.

```csharp
public VbaModuleCollection Modules { get; }
```

### Examples

```csharp
// Called: VbaModuleCollection modules = workbook.VbaProject.Modules;
[Test]
        public void Property_Modules()
        {
            
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.KeepUnparsedData = (false);
            loadOptions.ParsingFormulaOnOpen = (false);
            LoadFilter loadFilter = new LoadFilter(LoadDataFilterOptions.VBA);
            loadOptions.LoadFilter = (loadFilter);


            Workbook workbook = new Workbook(Constants.sourcePath + "CellsJava43196.xlsm", loadOptions);
            VbaModuleCollection modules = workbook.VbaProject.Modules;
            Assert.AreEqual(6,modules.Count);
        }
```

### See Also

* class [VbaModuleCollection](../../vbamodulecollection/)
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


