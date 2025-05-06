---
title: PageSetup.Copy
second_title: Aspose.Cells for .NET API Reference
description: PageSetup method. Copies the setting of the page setup
type: docs
url: /net/aspose.cells/pagesetup/copy/
---
## PageSetup.Copy method

Copies the setting of the page setup.

```csharp
public void Copy(PageSetup source, CopyOptions copyOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| source | PageSetup | The source. |
| copyOptions | CopyOptions | The copy options. |

### Examples

```csharp
// Called: destSheet.PageSetup.Copy(srcSheet.PageSetup, copyOptions);
static void Method_CopyOptions_(Workbook srcBook, Worksheet srcSheet, Workbook destBook,
            bool deleteIfAlreadyExists = true, bool removeFormulas = true)
        {
            if (deleteIfAlreadyExists)
                destBook.Worksheets.RemoveAt(srcSheet.Name);

            CopyOptions copyOptions = new CopyOptions();

            Worksheet destSheet = destBook.Worksheets.Add(srcSheet.Name);
            destSheet.Copy(srcSheet, copyOptions);

            // Copy the page setup from source to destination 
            destSheet.PageSetup.Copy(srcSheet.PageSetup, copyOptions);
            destSheet.PageSetup.PrintArea = srcSheet.PageSetup.PrintArea;
            destSheet.TabColor = srcSheet.TabColor;

            destBook.Worksheets.ExternalLinks.Clear(); //destBook.RemoveExternalLinks();

            if (removeFormulas)
                destSheet.Cells.RemoveFormulas();

            if (/*destBook.ContainsSheet(&quot;Sheet1&quot;) &amp;&amp; */destBook.Worksheets.Count &gt; 1)
                destBook.Worksheets.RemoveAt(&quot;Sheet1&quot;);
            //for (int i = destSheet.Charts.Count - 1; i &gt;= 7; i--)
            //{
            //   // if (destSheet.Charts[i].Type == ChartType.BoxWhisker)
            //    {
            //        destSheet.Charts.RemoveAt(i);
            //    }

            //}
            // destSheet.Charts.Clear();
            Util.ReSave(destBook, SaveFormat.Xlsm);
            //destBook.Save(Constants.destPath + &quot;CELLSNET46325.xlsm&quot;);
        }
```

### See Also

* class [CopyOptions](../../copyoptions/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


