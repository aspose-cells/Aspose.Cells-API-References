---
title: Cells.RemoveFormulas
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Removes all formula and replaces with the value of the formula
type: docs
url: /net/aspose.cells/cells/removeformulas/
---
## Cells.RemoveFormulas method

Removes all formula and replaces with the value of the formula.

```csharp
public void RemoveFormulas()
```

### Examples

```csharp
// Called: destSheet.Cells.RemoveFormulas();
static void Method_RemoveFormulas(Workbook srcBook, Worksheet srcSheet, Workbook destBook,
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

            if (/*destBook.ContainsSheet("Sheet1") && */destBook.Worksheets.Count > 1)
                destBook.Worksheets.RemoveAt("Sheet1");
            //for (int i = destSheet.Charts.Count - 1; i >= 7; i--)
            //{
            //   // if (destSheet.Charts[i].Type == ChartType.BoxWhisker)
            //    {
            //        destSheet.Charts.RemoveAt(i);
            //    }

            //}
            // destSheet.Charts.Clear();
            Util.ReSave(destBook, SaveFormat.Xlsm);
            //destBook.Save(Constants.destPath + "CELLSNET46325.xlsm");
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


