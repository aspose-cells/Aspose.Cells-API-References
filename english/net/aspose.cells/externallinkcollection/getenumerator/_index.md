---
title: ExternalLinkCollection.GetEnumerator
second_title: Aspose.Cells for .NET API Reference
description: ExternalLinkCollection method. Get an enumerator that iterates through this collection
type: docs
url: /net/aspose.cells/externallinkcollection/getenumerator/
---
## ExternalLinkCollection.GetEnumerator method

Get an enumerator that iterates through this collection.

```csharp
public IEnumerator GetEnumerator()
```

### Examples

```csharp
// Called: IEnumerator en = elc.GetEnumerator();
public void ExternalLinkCollection_Method_GetEnumerator()
{
    string[] funcs = new string[] { "customfunc1()", "customfunc1(1,2)", "customfunc2()", "customfunc2(3)" };
    Workbook wb = new Workbook();
    CreateExternalLinks(wb, funcs);

    ExternalLinkCollection elc = wb.Worksheets.ExternalLinks;
    Assert.AreEqual(4, elc.Count, "Count of existing external links");
    IEnumerator en = elc.GetEnumerator();
    for (int i = 0; i < 4; i++)
    {
        Assert.IsTrue(en.MoveNext(), "Enumerator should have next item");
        Assert.AreEqual("externallink" + (i + 1) + ".xlam",
            ((ExternalLink)en.Current).DataSource, "ExternalLink-" + i);
    }

    Cells cells = wb.Worksheets[0].Cells;
    for (int i = 0; i < 5; i++)
    {
        string el = "=externallink" + (i < 2 ? 1 : i) + ".xlam!";
        for (int j = 0; j < 4; j++)
        {
            Assert.AreEqual(el + funcs[j], cells[j, i].Formula,
                "Formula references to ExternalLink[" + i + "]-" + j);
        }
    }
    Assert.AreEqual("=[externallink1.xlam]Sheet1!$A$1", cells[0, 5].Formula,
        "Formula references to cell of ExternalLink[0]");
}
```

### See Also

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


