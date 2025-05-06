---
title: ListBox.PageChange
second_title: Aspose.Cells for .NET API Reference
description: ListBox property. Specifies the amount by which the controls value is changed when the user clicks on the scrollbars page up or page down region
type: docs
url: /net/aspose.cells.drawing/listbox/pagechange/
---
## ListBox.PageChange property

Specifies the amount by which the control's value is changed when the user clicks on the scrollbar's page up or page down region.

```csharp
public int PageChange { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(((ListBox)workbook.Worksheets[0].Shapes[0]).PageChange ,4);
[Test]
        public void Property_PageChange()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSJAVA41437.xlsx&quot;);
            Workbook _asposeWorkbook = new Workbook();
            _asposeWorkbook.Copy(workbook);
            Assert.AreEqual(((ListBox)workbook.Worksheets[0].Shapes[0]).PageChange ,4);
            _asposeWorkbook.Save(Constants.destPath +&quot;CELLSJAVA41437.xlsx&quot;);
        }
```

### See Also

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


