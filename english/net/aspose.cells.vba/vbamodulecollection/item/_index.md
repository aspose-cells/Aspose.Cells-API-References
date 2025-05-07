---
title: VbaModuleCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: VbaModuleCollection property. Gets VbaModule in the list by the index
type: docs
url: /net/aspose.cells.vba/vbamodulecollection/item/
---
## VbaModuleCollection indexer (1 of 2)

Gets [`VbaModule`](../../vbamodule/) in the list by the index.

```csharp
public VbaModule this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Examples

```csharp
// Called: workbook.VbaProject.Modules[i].Codes += " '" + i.ToString() + " ";
[Test]
        public void Property_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET43891.xlsm");
            Console.WriteLine("Before Deleting Sheet & Module: " + "workbook.Worksheets.Count: " + workbook.Worksheets.Count.ToString() + "workbook.VbaProject.Modules.Count: " + workbook.VbaProject.Modules.Count.ToString());
            workbook.Worksheets.RemoveAt(workbook.Worksheets.Count - 1);
            workbook.VbaProject.Modules.RemoveAt(workbook.VbaProject.Modules.Count - 1);
            Console.WriteLine("After Deleting Sheet & Module: " + "workbook.Worksheets.Count: " + workbook.Worksheets.Count.ToString() + "workbook.VbaProject.Modules.Count: " + workbook.VbaProject.Modules.Count.ToString());

            Console.WriteLine("Before Adding Sheet & Module: " + "workbook.Worksheets.Count: " + workbook.Worksheets.Count.ToString() + "workbook.VbaProject.Modules.Count: " + workbook.VbaProject.Modules.Count.ToString());
            workbook.VbaProject.Modules.Add(workbook.Worksheets.Add("TestSheet"));
            Console.WriteLine("After Adding Sheet & Module: " + "workbook.Worksheets.Count: " + workbook.Worksheets.Count.ToString() + "workbook.VbaProject.Modules.Count: " + workbook.VbaProject.Modules.Count.ToString());
            for (int i = 0; i <= workbook.VbaProject.Modules.Count - 1; i++)
            {
                workbook.VbaProject.Modules[i].Codes += " '" + i.ToString() + " ";
            }
            workbook.Save(Constants.destPath + "CELLSNET43891.xlsm");
            workbook = new Workbook(Constants.destPath + "CELLSNET43891.xlsm");
            Assert.AreEqual("Sheet1", workbook.Worksheets[0].CodeName);
        }
```

### See Also

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)

---

## VbaModuleCollection indexer (2 of 2)

Gets [`VbaModule`](../../vbamodule/) in the list by the name.

```csharp
public VbaModule this[string name] { get; }
```

| Parameter | Description |
| --- | --- |
| name | The name of module. |

### Examples

```csharp
// Called: lc_NewWorkBook.VbaProject.Modules[lc_Index].Codes = lc_WorkBook.VbaProject.Modules[lc_WorkBook.Worksheets["Controls"].CodeName].Codes;
[Test]
        public void Property_String_()
        {
            Workbook lc_WorkBook = new Workbook(Constants.sourcePath + "CellsNet53424.xlsm");
            Workbook lc_NewWorkBook = new Workbook();
            lc_NewWorkBook.Worksheets["Sheet1"].Copy(lc_WorkBook.Worksheets["Controls"]);


            //'VBAをコピーする
            int lc_Index = lc_NewWorkBook.VbaProject.Modules.Add(lc_NewWorkBook.Worksheets["Sheet1"]);
            lc_NewWorkBook.VbaProject.Modules[lc_Index].Codes = lc_WorkBook.VbaProject.Modules[lc_WorkBook.Worksheets["Controls"].CodeName].Codes;
           Assert.AreEqual("CommandButton1",lc_NewWorkBook.Worksheets[0].Shapes[0].Name);
            // 'ファイル名「Result.xlsm」で保存
            lc_NewWorkBook.Save(Constants.destPath + "CellsNet53424.xlsm", Aspose.Cells.SaveFormat.Xlsm);
            Assert.IsTrue(ManualFileUtil.ManualCheckStringInZip(Constants.destPath + "CellsNet53424.xlsm", "xl/worksheets/sheet1.xml", new string[] { "name=\"CommandButton1\"" }, true));
            Assert.IsTrue(ManualFileUtil.ManualCheckStringInZip(Constants.destPath + "CellsNet53424.xlsm", "xl/drawings/drawing1.xml", new string[] { "<xdr:cNvPr id=\"1027\"" }, true));
        }
```

### See Also

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


