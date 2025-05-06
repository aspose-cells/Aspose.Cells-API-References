---
title: Workbook.GetFonts
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Gets all fonts in the style pool
type: docs
url: /net/aspose.cells/workbook/getfonts/
---
## Workbook.GetFonts method

Gets all fonts in the style pool.

```csharp
public Font[] GetFonts()
```

### Examples

```csharp
// Called: int count = workbook.GetFonts().Length;
[Test]
        public void Method_GetFonts()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSJAVA42284.xlsx&quot;);
            Console.WriteLine(&quot;initial fonts &quot; + workbook.GetFonts().Length);
            int count = workbook.GetFonts().Length;
            {
                MemoryStream ms = new MemoryStream();
                workbook.Save(ms, new OoxmlSaveOptions(SaveFormat.Xlsx));
                byte[] bytes = ms.ToArray();
                workbook = new Workbook(new MemoryStream(bytes));
                Assert.AreEqual(count, workbook.GetFonts().Length);

            }
            {
                MemoryStream ms = new MemoryStream();
                workbook.Save(ms, new OoxmlSaveOptions(SaveFormat.Xlsx));
                byte[] bytes = ms.ToArray();
                workbook = new Workbook(new MemoryStream(bytes));
                Assert.AreEqual(count,workbook.GetFonts().Length);

            } 
        }
```

### See Also

* class [Font](../../font/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


