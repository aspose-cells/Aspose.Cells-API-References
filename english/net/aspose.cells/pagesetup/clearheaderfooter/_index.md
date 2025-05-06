---
title: PageSetup.ClearHeaderFooter
second_title: Aspose.Cells for .NET API Reference
description: PageSetup method. Clears header and footer setting
type: docs
url: /net/aspose.cells/pagesetup/clearheaderfooter/
---
## PageSetup.ClearHeaderFooter method

Clears header and footer setting.

```csharp
public void ClearHeaderFooter()
```

### Examples

```csharp
// Called: pageSetup.ClearHeaderFooter();
[Test]
        public void Method_ClearHeaderFooter()
        {
            Workbook workbook = new Workbook();
            var pageSetup = workbook.Worksheets[0].PageSetup;

            //This line causes NullReferenceException when setting either Header or Footer below
            pageSetup.ClearHeaderFooter();

            pageSetup.SetHeader(0, &quot;Left Header&quot;);
            pageSetup.SetFooter(0, &quot;Left Footer&quot;);

            
        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


