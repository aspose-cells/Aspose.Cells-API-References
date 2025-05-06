---
title: WriteProtection.IsWriteProtected
second_title: Aspose.Cells for .NET API Reference
description: WriteProtection property. Indicates whether this workbook is write protected
type: docs
url: /net/aspose.cells/writeprotection/iswriteprotected/
---
## WriteProtection.IsWriteProtected property

Indicates whether this workbook is write protected.

```csharp
public bool IsWriteProtected { get; }
```

### Examples

```csharp
// Called: Console.WriteLine(wb.Settings.WriteProtection.IsWriteProtected.ToString());//True --&amp;gt; Issue
[Test]
        //http://www.aspose.com/community/forums/thread/335406.aspx
        public void Property_IsWriteProtected()
        {
            Console.WriteLine(&quot;testCELLSNET_31277()&quot;);
            string infn = path + @&quot;CELLSNET-31277/Test.xlsx&quot;;
            string outfn = destpath + @&quot;Test.out.xlsx&quot;;
            Workbook wb = new Workbook(infn);
            Console.WriteLine(wb.Settings.WriteProtection.IsWriteProtected.ToString()); //False --&gt; OK
            Assert.AreEqual(wb.Settings.WriteProtection.IsWriteProtected, false);
            wb.Save(outfn);

            wb = new Workbook(outfn);
            Console.WriteLine(wb.Settings.WriteProtection.IsWriteProtected.ToString());//True --&gt; Issue
            Assert.AreEqual(wb.Settings.WriteProtection.IsWriteProtected, false);
        }
```

### See Also

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


