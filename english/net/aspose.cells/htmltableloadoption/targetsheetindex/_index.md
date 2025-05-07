---
title: HtmlTableLoadOption.TargetSheetIndex
second_title: Aspose.Cells for .NET API Reference
description: HtmlTableLoadOption property. Get or set the target index of worksheet where the table is to be located
type: docs
url: /net/aspose.cells/htmltableloadoption/targetsheetindex/
---
## HtmlTableLoadOption.TargetSheetIndex property

Get or set the target index of worksheet where the table is to be located.

```csharp
public int TargetSheetIndex { get; set; }
```

### Examples

```csharp
// Called: tableLoadOption.TargetSheetIndex = 1;
[Test]
        public void Property_TargetSheetIndex()
        {
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.SupportDivTag = true;
            loadOptions.LoadFilter.LoadDataFilterOptions = LoadDataFilterOptions.Chart;
            loadOptions.TableLoadOptions.Add(1);
            loadOptions.TableLoadOptions.Add(2);
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "id5";
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "id6";
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            Workbook wb = new Workbook(Constants.HtmlPath + "HtmlTableLoadOption.htm", loadOptions);
            wb.Save(_destFilesPath + "HtmlTableLoadOption1.xlsx");
            Assert.AreEqual("222aaa", wb.Worksheets[0].Cells["A1"].StringValue);
            Assert.AreEqual("333aaa", wb.Worksheets[0].Cells["A2"].StringValue);
            Assert.AreEqual("555aaa", wb.Worksheets[0].Cells["A4"].StringValue);
            Assert.AreEqual("666aaa", wb.Worksheets[0].Cells["A7"].StringValue);

            loadOptions.TableLoadOptions.Clear();
            loadOptions.TableLoadOptions.Add(0, 2);
            loadOptions.TableLoadOptions.Add(1, 0);
            loadOptions.TableLoadOptions.Add(2, 1);
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "id5";
            tableLoadOption.TargetSheetIndex= 0;
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "id6";
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            tableLoadOption.TargetSheetIndex = 1;
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "id4";
            tableLoadOption.TargetSheetIndex = 2;
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            wb = new Workbook(Constants.HtmlPath + "HtmlTableLoadOption.htm", loadOptions);
            wb.Save(_destFilesPath + "HtmlTableLoadOption2.xlsx");
            Assert.AreEqual("222bbb", wb.Worksheets[0].Cells["B1"].StringValue);
            Assert.AreEqual("555bbb", wb.Worksheets[0].Cells["B2"].StringValue);
            Assert.AreEqual("333bbb", wb.Worksheets[1].Cells["B1"].StringValue);
            Assert.AreEqual("666bbb", wb.Worksheets[1].Cells["B3"].StringValue);
            Assert.AreEqual("111ccc", wb.Worksheets[2].Cells["C1"].StringValue);
            Assert.AreEqual("444ccc", wb.Worksheets[2].Cells["C2"].StringValue);
        }
```

### See Also

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


