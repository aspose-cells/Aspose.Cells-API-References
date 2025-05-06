---
title: LoadOptions.MemorySetting
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. Gets or sets the memory usage options
type: docs
url: /net/aspose.cells/loadoptions/memorysetting/
---
## LoadOptions.MemorySetting property

Gets or sets the memory usage options.

```csharp
public MemorySetting MemorySetting { get; set; }
```

### Examples

```csharp
// Called: new LoadOptions() { MemorySetting = MemorySetting.MemoryPreference });
[Test]
        public void Property_MemorySetting()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;xlsb/CELLSNET-51195.xlsb&quot;,
                new LoadOptions() { MemorySetting = MemorySetting.MemoryPreference });
            Cells cells = wb.Worksheets[0].Cells;
            Assert.AreEqual(&quot;{=TABLE(,B3)}&quot;, cells[2, 3].Formula, &quot;D3.Formula&quot;);
            Assert.AreEqual(&quot;{=TABLE(,B3)}&quot;, cells[3, 3].Formula, &quot;D4.Formula&quot;);
            Assert.AreEqual(&quot;{=TABLE(,B3)}&quot;, cells[4, 3].Formula, &quot;D5.Formula&quot;);
            Assert.AreEqual(1.0, cells[2, 3].DoubleValue, &quot;D3.Value&quot;);
            Assert.AreEqual(&quot;a&quot;, cells[3, 3].Value, &quot;D4.Value&quot;);
            Assert.AreEqual(0.03, cells[4, 3].DoubleValue, &quot;D5.Value&quot;);
            foreach (SaveFormat sf in new SaveFormat[] { SaveFormat.Xlsx, SaveFormat.Excel97To2003, SaveFormat.Xlsb, })
            {
                wb = Util.ReSave(wb, sf);
                cells = wb.Worksheets[0].Cells;
                for (int i = 2; i &lt; 5; i++)
                {
                    Assert.AreEqual(&quot;{=TABLE(,B3)}&quot;, cells[2, 3].Formula, sf + &quot;-D3.Formula&quot;);
                    Assert.AreEqual(&quot;{=TABLE(,B3)}&quot;, cells[3, 3].Formula, sf + &quot;-D4.Formula&quot;);
                    Assert.AreEqual(&quot;{=TABLE(,B3)}&quot;, cells[4, 3].Formula, sf + &quot;-D5.Formula&quot;);
                    Assert.AreEqual(1.0, cells[2, 3].DoubleValue, sf + &quot;-D3.Value&quot;);
                    Assert.AreEqual(&quot;a&quot;, cells[3, 3].Value, sf + &quot;-D4.Value&quot;);
                    Assert.AreEqual(0.03, cells[4, 3].DoubleValue, sf + &quot;-D5.Value&quot;);
                }
            }
        }
```

### See Also

* enum [MemorySetting](../../memorysetting/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


