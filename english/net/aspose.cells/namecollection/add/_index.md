---
title: NameCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: NameCollection method. Defines a new name
type: docs
url: /net/aspose.cells/namecollection/add/
---
## NameCollection.Add method

Defines a new name.

```csharp
public int Add(string text)
```

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | The text to use as the name. |

### Return Value

[`Name`](../../name/) object index.

### Remarks

Name cannot include spaces and cannot look like cell references.

### Examples

```csharp
// Called: wb.Worksheets.Names[wb.Worksheets.Names.Add("testname")].RefersTo = "=[Book1.xlsx]Sheet1!$A1";
[Test]
        public void Method_String_()
        {
            Workbook wb = new Workbook();
            wb.Worksheets.Add("Sheet2");
            wb.Worksheets.Add("Sheet3");
            wb.Worksheets.Names[wb.Worksheets.Names.Add("testname")].RefersTo = "=[Book1.xlsx]Sheet1!$A1";
            wb.Worksheets.Names[wb.Worksheets.Names.Add("Sheet2!testname")].RefersTo = "=[Book1.xlsx]Sheet2!$A2";
            wb.Worksheets[1].Cells[0, 0].SetSharedFormula("=testname", 10, 1);
            wb.Worksheets[2].Cells[0, 0].SetSharedFormula("=testname", 10, 1);
            wb.Worksheets.Add();
            wb.Worksheets.ExternalLinks.Clear();
            wb.Worksheets.RemoveAt("Sheet1");
            wb.Worksheets.RemoveAt("Sheet2");
            wb.Worksheets.RemoveAt("Sheet3");
            wb.Save(new MemoryStream(), SaveFormat.Xlsx);
        }
```

### See Also

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


