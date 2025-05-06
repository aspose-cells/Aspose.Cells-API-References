---
title: Enum HtmlCrossType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.HtmlCrossType enum. Represents five types of html cross string
type: docs
url: /net/aspose.cells/htmlcrosstype/
---
## HtmlCrossType enumeration

Represents five types of html cross string.

```csharp
public enum HtmlCrossType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Default | `0` | Display like MS Excel,depends on the next cell. If the next cell is null,the string will cross,or it will be truncated |
| MSExport | `1` | Display the string like MS Excel exporting html. |
| Cross | `2` | Display HTML cross string, this performance for creating large html files will be more than ten times faster than setting the value to Default or FitToCell. |
| CrossHideRight | `3` | Display HTML cross string and hide the right string when the texts overlap. |
| FitToCell | `4` | Only displaying the string within the width of cell. |

### Examples

```csharp
// Called: options.HtmlCrossStringType = HtmlCrossType.Cross;
[Test]
        public void Type_HtmlCrossType()
        {
            

            Workbook wb = new Workbook(Constants.sourcePath + &quot;NET46496.xlsx&quot;);
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.HtmlCrossStringType = HtmlCrossType.Default;
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, options);
                string text = Encoding.UTF8.GetString(ms.GetBuffer(), 0, (int)ms.Length);
                Assert.IsTrue(text.IndexOf(&quot;&lt;td colspan=&apos;2&apos; style=&apos;mso-ignore:colspan;overflow:hidden;&apos;&gt;This is a sample string. This is a sample string.&lt;/td&gt;&quot;) != -1);
            }

            options.HtmlCrossStringType = HtmlCrossType.MSExport;
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, options);
                string text = Encoding.UTF8.GetString(ms.GetBuffer(), 0, (int)ms.Length);
                Assert.IsTrue(text.IndexOf(&quot;&lt;td&gt;This is a sample string.&amp;nbsp;&lt;span style=&apos;display:none&apos;&gt;This is a sample string.&lt;/span&gt;&lt;/td&gt;&quot;) != -1);
            }
            options.HtmlCrossStringType = HtmlCrossType.FitToCell;
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, options);
                string text = Encoding.UTF8.GetString(ms.GetBuffer(), 0, (int)ms.Length);
                Assert.IsTrue(text.IndexOf(&quot;&lt;td style=&apos;overflow:hidden;&apos;&gt;This is a sample string. This is a sample string.&lt;/td&gt;&quot;) != -1);
            }


            options.HtmlCrossStringType = HtmlCrossType.Cross;
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, options);
                string text = Encoding.UTF8.GetString(ms.GetBuffer(), 0, (int)ms.Length);
                Assert.IsTrue(text.IndexOf(&quot;&lt;td colspan=&apos;2&apos; style=&apos;mso-ignore:colspan;&apos;&gt;This is a sample string. This is a sample string.&lt;/td&gt;&quot;) != -1);
            }
            options.HtmlCrossStringType = HtmlCrossType.CrossHideRight;
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, options);
                string text = Encoding.UTF8.GetString(ms.GetBuffer(), 0, (int)ms.Length);
                Assert.IsTrue(text.IndexOf(&quot;&lt;td style=&apos;visibility:hidden;&apos;&gt;&amp;nbsp;Test2&lt;/td&gt;&quot;) != -1);
            }
        }
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


