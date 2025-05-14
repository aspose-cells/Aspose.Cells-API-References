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
// Called: Name n = wb.Worksheets.Names[wb.Worksheets.Names.Add("REFERSTO")];
public void NameCollection_Method_Add()
{
    Workbook wb = new Workbook(FileFormatType.Xlsx);
    Name n = wb.Worksheets.Names[wb.Worksheets.Names.Add("REFERSTO")];
    string fml = "=OFFSET(Sheet1!XEV1,0,0,ROW(Sheet1!XEV17)-ROW(Sheet1!XEV1)+1,COLUMN(Sheet1!XFC1)-COLUMN(Sheet1!XEV1)+1)";
    n.RefersTo = fml;
    Assert.AreEqual(fml, n.RefersTo, "RefersTo based on A1");
    Aspose.Cells.Range r = n.GetRange(0, 0, 0);
    Assert.AreEqual("XEV1:XFC17", r.Address, "Range.Address based on A1");

  //  Assert.AreEqual("=OFFSET(Sheet1!D7,0,0,ROW(Sheet1!D23)-ROW(Sheet1!D7)+1,COLUMN(Sheet1!K7)-COLUMN(Sheet1!D7)+1)",
     //   n.GetRefersTo(false, false, 6, 12), "RefersTo based on M7");
 //   r = n.GetRange(0, 6, 12);
  //  Assert.AreEqual("D7:K23", r.Address, "Range.Address based on M7");
}
```

### See Also

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


