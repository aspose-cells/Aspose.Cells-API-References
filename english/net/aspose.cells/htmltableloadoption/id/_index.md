---
title: HtmlTableLoadOption.Id
second_title: Aspose.Cells for .NET API Reference
description: HtmlTableLoadOption property. Get or set the id of table to import from html
type: docs
url: /net/aspose.cells/htmltableloadoption/id/
---
## HtmlTableLoadOption.Id property

Get or set the id of table to import from html

```csharp
public string Id { get; set; }
```

### Examples

```csharp
// Called: tableLoadOption.Id = &amp;quot;id5&amp;quot;;
[Test]
        public void Property_Id()
        {
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.SupportDivTag = true;
            loadOptions.LoadFilter.LoadDataFilterOptions = LoadDataFilterOptions.Chart;
            loadOptions.TableLoadOptions.Add(1);
            loadOptions.TableLoadOptions.Add(2);
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = &quot;id5&quot;;
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = &quot;id6&quot;;
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            Workbook wb = new Workbook(Constants.HtmlPath + &quot;HtmlTableLoadOption.htm&quot;, loadOptions);
            wb.Save(_destFilesPath + &quot;HtmlTableLoadOption1.xlsx&quot;);
            Assert.AreEqual(&quot;222aaa&quot;, wb.Worksheets[0].Cells[&quot;A1&quot;].StringValue);
            Assert.AreEqual(&quot;333aaa&quot;, wb.Worksheets[0].Cells[&quot;A2&quot;].StringValue);
            Assert.AreEqual(&quot;555aaa&quot;, wb.Worksheets[0].Cells[&quot;A4&quot;].StringValue);
            Assert.AreEqual(&quot;666aaa&quot;, wb.Worksheets[0].Cells[&quot;A7&quot;].StringValue);

            loadOptions.TableLoadOptions.Clear();
            loadOptions.TableLoadOptions.Add(0, 2);
            loadOptions.TableLoadOptions.Add(1, 0);
            loadOptions.TableLoadOptions.Add(2, 1);
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = &quot;id5&quot;;
            tableLoadOption.TargetSheetIndex= 0;
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = &quot;id6&quot;;
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            tableLoadOption.TargetSheetIndex = 1;
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = &quot;id4&quot;;
            tableLoadOption.TargetSheetIndex = 2;
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            wb = new Workbook(Constants.HtmlPath + &quot;HtmlTableLoadOption.htm&quot;, loadOptions);
            wb.Save(_destFilesPath + &quot;HtmlTableLoadOption2.xlsx&quot;);
            Assert.AreEqual(&quot;222bbb&quot;, wb.Worksheets[0].Cells[&quot;B1&quot;].StringValue);
            Assert.AreEqual(&quot;555bbb&quot;, wb.Worksheets[0].Cells[&quot;B2&quot;].StringValue);
            Assert.AreEqual(&quot;333bbb&quot;, wb.Worksheets[1].Cells[&quot;B1&quot;].StringValue);
            Assert.AreEqual(&quot;666bbb&quot;, wb.Worksheets[1].Cells[&quot;B3&quot;].StringValue);
            Assert.AreEqual(&quot;111ccc&quot;, wb.Worksheets[2].Cells[&quot;C1&quot;].StringValue);
            Assert.AreEqual(&quot;444ccc&quot;, wb.Worksheets[2].Cells[&quot;C2&quot;].StringValue);
        }
```

### See Also

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


