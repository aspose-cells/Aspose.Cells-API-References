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
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet42963.xlsx&quot;);
            Assert.AreEqual(&quot;=&apos;C:/Users/Leonid_Veriga/AppData/Roaming/Microsoft/AddIns/AI1.xlam&apos;!test1(1)&quot;,
                workbook.Worksheets[0].Cells[&quot;A3&quot;].Formula.Replace(&apos;\\&apos;, &apos;/&apos;));
            ExternalLinkCollection elc = workbook.Worksheets.ExternalLinks;
            Assert.AreEqual(2, elc.Count);
            for (int i = elc.Count - 1; i &gt; -1; i--)
            {
                if (elc[i].DataSource.IndexOf(&quot;AddIns&quot;) &lt; 0)
                {
                    elc.RemoveAt(i);
                }
            }
            Assert.AreEqual(1, elc.Count);
            Assert.AreEqual(workbook.Worksheets[0].Cells[&quot;A3&quot;].IsFormula, true);
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
private void Method_Boolean_(bool updateReferences)
        {
            string[] funcs = new string[] { &quot;customfunc1()&quot;, &quot;customfunc1(1,2)&quot;, &quot;customfunc2()&quot;, &quot;customfunc2(3)&quot; };
            Workbook wb = new Workbook();
            CreateExternalLinks(wb, funcs);
            ExternalLinkCollection elc = wb.Worksheets.ExternalLinks;

            elc.RemoveAt(1, updateReferences);
            Assert.AreEqual(3, elc.Count, &quot;Count of external links after remove&quot;);
            IEnumerator en = elc.GetEnumerator();
            for (int i = 0; i &lt; 3; i++)
            {
                Assert.IsTrue(en.MoveNext(), &quot;Enumerator should have next item&quot;);
                Assert.AreEqual(&quot;externallink&quot; + (i == 0 ? 1 : i + 2) + &quot;.xlam&quot;,
                    ((ExternalLink)en.Current).DataSource, &quot;ExternalLink-&quot; + i);
            }
            Cells cells = wb.Worksheets[0].Cells;
            for (int i = 0; i &lt; 5; i++)
            {
                if (i == 2)
                {
                    for (int j = 0; j &lt; 4; j++)
                    {
                        if (updateReferences)
                        {
                            Assert.AreEqual(&quot;=&quot; + funcs[j], cells[j, i].Formula,
                                &quot;Formula references to ExternalLink[&quot; + i + &quot;]-&quot; + j);
                        }
                        else
                        {
                            Assert.IsFalse(cells[j, i].IsFormula, i + &quot;-&quot; + j + &quot;&apos;s formula should have been removed&quot;);
                        }
                    }
                }
                else
                {
                    string el = &quot;=externallink&quot; + (i &lt; 2 ? 1 : i) + &quot;.xlam!&quot;;
                    for (int j = 0; j &lt; 4; j++)
                    {
                        Assert.AreEqual(el + funcs[j], cells[j, i].Formula,
                            &quot;Formula references to ExternalLink[&quot; + i + &quot;]-&quot; + j);
                    }
                }
            }
            Assert.AreEqual(&quot;=[externallink1.xlam]Sheet1!$A$1&quot;, cells[0, 5].Formula,
                &quot;Formula references to cell of ExternalLink[0]&quot;);

            elc.RemoveAt(0, updateReferences);
            Assert.AreEqual(2, elc.Count, &quot;Count of external links after remove&quot;);
            en = elc.GetEnumerator();
            for (int i = 0; i &lt; 2; i++)
            {
                Assert.IsTrue(en.MoveNext(), &quot;Enumerator should have next item&quot;);
                Assert.AreEqual(&quot;externallink&quot; + (i + 3) + &quot;.xlam&quot;,
                    ((ExternalLink)en.Current).DataSource, &quot;ExternalLink-&quot; + i);
            }
            for (int i = 0; i &lt; 3; i++)
            {
                for (int j = 0; j &lt; 4; j++)
                {
                    if (updateReferences)
                    {
                        Assert.AreEqual(&quot;=&quot; + funcs[j], cells[j, i].Formula,
                            &quot;Formula references to ExternalLink[&quot; + i + &quot;]-&quot; + j);
                    }
                    else
                    {
                        Assert.IsFalse(cells[j, i].IsFormula, i + &quot;-&quot; + j + &quot;&apos;s formula should have been removed&quot;);
                    }
                }
            }
            for (int i = 3; i &lt; 5; i++)
            {
                string el = &quot;=externallink&quot; + i + &quot;.xlam!&quot;;
                for (int j = 0; j &lt; 4; j++)
                {
                    Assert.AreEqual(el + funcs[j], cells[j, i].Formula,
                        &quot;Formula references to ExternalLink[&quot; + i + &quot;]-&quot; + j);
                }
            }
            if (updateReferences)
            {
                Assert.AreEqual(&quot;=Sheet1!$A$1&quot;, cells[0, 5].Formula,
                    &quot;Formula references to cell of ExternalLink[0]&quot;);
                Assert.AreEqual(&quot;=#REF!$A$1&quot;, cells[0, 6].Formula,
                    &quot;Formula references to cell of ExternalLink[0]&quot;);
            }
            else
            {
                Assert.IsFalse(cells[0, 5].IsFormula, &quot;0-5&apos;s formula should have been removed&quot;);
                Assert.IsFalse(cells[0, 6].IsFormula, &quot;0-6&apos;s formula should have been removed&quot;);
            }
        }
```

### See Also

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


