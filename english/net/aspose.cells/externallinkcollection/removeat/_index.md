---
title: ExternalLinkCollection.RemoveAt
second_title: Aspose.Cells for .NET API Reference
description: ExternalLinkCollection method. Removes the specified external link from the workbook
type: docs
url: /net/aspose.cells/externallinkcollection/removeat/
---
## RemoveAt(int) {#removeat}

Removes the specified external link from the workbook.

```csharp
public void RemoveAt(int index)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | the index of the external link to be removed. |

### Remarks

When removing the external link, all formulas that reference to it will be removed too because the references become invalid.

### Examples

```csharp
// Called: elc.RemoveAt(i);
public void ExternalLinkCollection_Method_RemoveAt()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Assert.AreEqual("='C:/Users/Leonid_Veriga/AppData/Roaming/Microsoft/AddIns/AI1.xlam'!test1(1)",
        workbook.Worksheets[0].Cells["A3"].Formula.Replace('\\', '/'));
    ExternalLinkCollection elc = workbook.Worksheets.ExternalLinks;
    Assert.AreEqual(2, elc.Count);
    for (int i = elc.Count - 1; i > -1; i--)
    {
        if (elc[i].DataSource.IndexOf("AddIns") < 0)
        {
            elc.RemoveAt(i);
        }
    }
    Assert.AreEqual(1, elc.Count);
    Assert.AreEqual(workbook.Worksheets[0].Cells["A3"].IsFormula, true);
}
```

### See Also

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveAt(int, bool) {#removeat_1}

Removes the specified external link from the workbook.

```csharp
public void RemoveAt(int index, bool updateReferencesAsLocal)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | the index of the external link to be removed. |
| updateReferencesAsLocal | Boolean | Whether update all references of given external link to reference of current workbook itself. Check [`Clear`](../clear/) to get more details about this parameter. |

### Examples

```csharp
// Called: elc.RemoveAt(0, updateReferences);
private void ExternalLinkCollection_Method_RemoveAt(bool updateReferences)
        {
            string[] funcs = new string[] { "customfunc1()", "customfunc1(1,2)", "customfunc2()", "customfunc2(3)" };
            Workbook wb = new Workbook();
            CreateExternalLinks(wb, funcs);
            ExternalLinkCollection elc = wb.Worksheets.ExternalLinks;

            elc.RemoveAt(1, updateReferences);
            Assert.AreEqual(3, elc.Count, "Count of external links after remove");
            IEnumerator en = elc.GetEnumerator();
            for (int i = 0; i < 3; i++)
            {
                Assert.IsTrue(en.MoveNext(), "Enumerator should have next item");
                Assert.AreEqual("externallink" + (i == 0 ? 1 : i + 2) + ".xlam",
                    ((ExternalLink)en.Current).DataSource, "ExternalLink-" + i);
            }
            Cells cells = wb.Worksheets[0].Cells;
            for (int i = 0; i < 5; i++)
            {
                if (i == 2)
                {
                    for (int j = 0; j < 4; j++)
                    {
                        if (updateReferences)
                        {
                            Assert.AreEqual("=" + funcs[j], cells[j, i].Formula,
                                "Formula references to ExternalLink[" + i + "]-" + j);
                        }
                        else
                        {
                            Assert.IsFalse(cells[j, i].IsFormula, i + "-" + j + "'s formula should have been removed");
                        }
                    }
                }
                else
                {
                    string el = "=externallink" + (i < 2 ? 1 : i) + ".xlam!";
                    for (int j = 0; j < 4; j++)
                    {
                        Assert.AreEqual(el + funcs[j], cells[j, i].Formula,
                            "Formula references to ExternalLink[" + i + "]-" + j);
                    }
                }
            }
            Assert.AreEqual("=[externallink1.xlam]Sheet1!$A$1", cells[0, 5].Formula,
                "Formula references to cell of ExternalLink[0]");

            elc.RemoveAt(0, updateReferences);
            Assert.AreEqual(2, elc.Count, "Count of external links after remove");
            en = elc.GetEnumerator();
            for (int i = 0; i < 2; i++)
            {
                Assert.IsTrue(en.MoveNext(), "Enumerator should have next item");
                Assert.AreEqual("externallink" + (i + 3) + ".xlam",
                    ((ExternalLink)en.Current).DataSource, "ExternalLink-" + i);
            }
            for (int i = 0; i < 3; i++)
            {
                for (int j = 0; j < 4; j++)
                {
                    if (updateReferences)
                    {
                        Assert.AreEqual("=" + funcs[j], cells[j, i].Formula,
                            "Formula references to ExternalLink[" + i + "]-" + j);
                    }
                    else
                    {
                        Assert.IsFalse(cells[j, i].IsFormula, i + "-" + j + "'s formula should have been removed");
                    }
                }
            }
            for (int i = 3; i < 5; i++)
            {
                string el = "=externallink" + i + ".xlam!";
                for (int j = 0; j < 4; j++)
                {
                    Assert.AreEqual(el + funcs[j], cells[j, i].Formula,
                        "Formula references to ExternalLink[" + i + "]-" + j);
                }
            }
            if (updateReferences)
            {
                Assert.AreEqual("=Sheet1!$A$1", cells[0, 5].Formula,
                    "Formula references to cell of ExternalLink[0]");
                Assert.AreEqual("=#REF!$A$1", cells[0, 6].Formula,
                    "Formula references to cell of ExternalLink[0]");
            }
            else
            {
                Assert.IsFalse(cells[0, 5].IsFormula, "0-5's formula should have been removed");
                Assert.IsFalse(cells[0, 6].IsFormula, "0-6's formula should have been removed");
            }
        }
```

### See Also

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


