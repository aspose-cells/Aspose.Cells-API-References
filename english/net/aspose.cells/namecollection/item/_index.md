---
title: NameCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: NameCollection property. Gets the Name element at the specified index
type: docs
url: /net/aspose.cells/namecollection/item/
---
## NameCollection indexer (1 of 2)

Gets the [`Name`](../../name/) element at the specified index.

```csharp
public Name this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
// Called: Assert.AreEqual("=Sheet3!$C$3:$E$6", workbook.Worksheets.Names[1].RefersTo);
public void NameCollection_Property_Item()
{
           
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    // workbook.Worksheets.RemoveAt(1);
    Assert.AreEqual("=#REF!A1",workbook.Worksheets[0].Cells["B2"].Formula);
    Assert.AreEqual("=#REF!$C$3:$E$8", workbook.Worksheets.Names[0].RefersTo);
    Assert.AreEqual("=Sheet3!$C$3:$E$6", workbook.Worksheets.Names[1].RefersTo);
    workbook.Save(Constants.destPath + "example.ods");
    workbook = new Workbook(Constants.destPath + "example.ods");
    Assert.AreEqual("=#REF!", workbook.Worksheets[0].Cells["B2"].Formula);
    Assert.AreEqual("=#REF!", workbook.Worksheets.Names[0].RefersTo);
    Assert.AreEqual("=Sheet3!$C$3:$E$6", workbook.Worksheets.Names[1].RefersTo);
    using (FileStream fs = File.OpenRead(Constants.destPath + "example.ods"))
    {
        ZipFile zipFile = ZipFile.Read(fs);
        ZipEntry en = zipFile.GetEntry("content.xml");
        System.IO.Stream s = zipFile.GetInputStream(en);
        StreamReader rdr = new StreamReader(s, Encoding.UTF8);
        String text = rdr.ReadToEnd();
        Assert.AreEqual(-1, text.IndexOf("#REF!#REF!"));
    }
}
```

### See Also

* class [Name](../../name/)
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## NameCollection indexer (2 of 2)

Gets the [`Name`](../../name/) element with the specified name.

```csharp
public Name this[string text] { get; }
```

| Parameter | Description |
| --- | --- |
| text | Name text. |

### Return Value

The element with the specified name.

### Examples

```csharp
// Called: Name name = names[text];
public override void NameCollection_Property_Item(CalculationData data)
            {
                if (data.FunctionName == "MYFUNC")
                {
                    string text = data.GetParamText(0);
                    Name name = names[text];
                    if (name == null)
                    {
                        Assert.Fail("Cannot get corresponding Name object of " + text);
                    }
                    ProcessNamesForPerf(sn % 10 == 0 ? text + ": " : null, names, false);
                    data.CalculatedValue = sn;
                    sn++;
                }
            }
```

### See Also

* class [Name](../../name/)
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


