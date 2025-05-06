---
title: ExternalLinkCollection.Clear
second_title: Aspose.Cells for .NET API Reference
description: ExternalLinkCollection method. Removes all external links
type: docs
url: /net/aspose.cells/externallinkcollection/clear/
---
## Clear() {#clear}

Removes all external links.

```csharp
public void Clear()
```

### Remarks

When removing external links, all formulas that reference to them will be removed too because the references become invalid.

### Examples

```csharp
// Called: workbook.Worksheets.ExternalLinks.Clear(); //workbook.RemoveExternalLinks();
[Test]
        public void Method_Clear()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNETCORE-97.xlsx&quot;);
            workbook.Worksheets.ExternalLinks.Clear(); //workbook.RemoveExternalLinks();
            workbook.Save(Constants.destPath + &quot;CELLSNETCORE-97.xlsx&quot;);
        }
```

### See Also

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Clear(bool) {#clear_1}

Removes all external links.

```csharp
public void Clear(bool updateReferencesAsLocal)
```

| Parameter | Type | Description |
| --- | --- | --- |
| updateReferencesAsLocal | Boolean | Whether update all references of external links in formulas to references of current workbook itself. |

### Remarks

If references are required to be updated, those references of external links in formulas will be changed to current workbook when it is possible. For example, one cell's original formula is "='externalsource.xlam'!customfunction()", after removing external links, the formula will become "=customfunction()"; When the original formula is "='[externalsource.xlam]Sheet1'!$A$1", according to whether there is one sheet with name "Sheet1" in current workbook: if true, the formula will become "=Sheet1!$A$1"; if false, the formula will become "=#REF!$A$1". If references are not required to be updated, all formulas with references to external links will be removed too because those references become invalid.

### Examples

```csharp
// Called: elc.Clear(updateReferences);
private void Method_Boolean_(bool updateReferences)
        {
            string[] funcs = new string[] { &quot;customfunc1()&quot;, &quot;customfunc1(1,2)&quot;, &quot;customfunc2()&quot;, &quot;customfunc2(3)&quot; };
            Workbook wb = new Workbook();
            CreateExternalLinks(wb, funcs);
            ExternalLinkCollection elc = wb.Worksheets.ExternalLinks;
            elc.Clear(updateReferences);

            Assert.AreEqual(0, elc.Count, &quot;Count of external links after clear&quot;);
            Cells cells = wb.Worksheets[0].Cells;
            for (int i = 0; i &lt; 5; i++)
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


