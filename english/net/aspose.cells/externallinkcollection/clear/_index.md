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
            Workbook workbook = new Workbook();
            VbaProject p = workbook.VbaProject;
            AddResource(workbook, "CELLSNET48746.cls");
            workbook.Worksheets.ExternalLinks.Clear(); //workbook.RemoveExternalLinks();
            workbook.Save(Constants.destPath + "CELLSNET48746.xlsm");
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
            string[] funcs = new string[] { "customfunc1()", "customfunc1(1,2)", "customfunc2()", "customfunc2(3)" };
            Workbook wb = new Workbook();
            CreateExternalLinks(wb, funcs);
            ExternalLinkCollection elc = wb.Worksheets.ExternalLinks;
            elc.Clear(updateReferences);

            Assert.AreEqual(0, elc.Count, "Count of external links after clear");
            Cells cells = wb.Worksheets[0].Cells;
            for (int i = 0; i < 5; i++)
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


