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
[Test]
        public void Method_GetEnumerator()
        {
            string[] funcs = new string[] { &quot;customfunc1()&quot;, &quot;customfunc1(1,2)&quot;, &quot;customfunc2()&quot;, &quot;customfunc2(3)&quot; };
            Workbook wb = new Workbook();
            CreateExternalLinks(wb, funcs);

            ExternalLinkCollection elc = wb.Worksheets.ExternalLinks;
            Assert.AreEqual(4, elc.Count, &quot;Count of existing external links&quot;);
            IEnumerator en = elc.GetEnumerator();
            for (int i = 0; i &lt; 4; i++)
            {
                Assert.IsTrue(en.MoveNext(), &quot;Enumerator should have next item&quot;);
                Assert.AreEqual(&quot;externallink&quot; + (i + 1) + &quot;.xlam&quot;,
                    ((ExternalLink)en.Current).DataSource, &quot;ExternalLink-&quot; + i);
            }

            Cells cells = wb.Worksheets[0].Cells;
            for (int i = 0; i &lt; 5; i++)
            {
                string el = &quot;=externallink&quot; + (i &lt; 2 ? 1 : i) + &quot;.xlam!&quot;;
                for (int j = 0; j &lt; 4; j++)
                {
                    Assert.AreEqual(el + funcs[j], cells[j, i].Formula,
                        &quot;Formula references to ExternalLink[&quot; + i + &quot;]-&quot; + j);
                }
            }
            Assert.AreEqual(&quot;=[externallink1.xlam]Sheet1!$A$1&quot;, cells[0, 5].Formula,
                &quot;Formula references to cell of ExternalLink[0]&quot;);
        }
```

### See Also

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


