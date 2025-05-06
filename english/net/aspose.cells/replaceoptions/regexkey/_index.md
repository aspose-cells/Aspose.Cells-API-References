---
title: ReplaceOptions.RegexKey
second_title: Aspose.Cells for .NET API Reference
description: ReplaceOptions property. Indicates whether the searched key is regex. If true then the searched key will be taken as regex
type: docs
url: /net/aspose.cells/replaceoptions/regexkey/
---
## ReplaceOptions.RegexKey property

Indicates whether the searched key is regex. If true then the searched key will be taken as regex.

```csharp
public bool RegexKey { get; set; }
```

### Examples

```csharp
// Called: opts.RegexKey = true;
[Test]
        public void Property_RegexKey()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            string[] src = new string[]
            {
                &quot;KIM&quot;, &quot;rONNIE CALLED KIM AND KIMINFORMED KIM  HER.&quot;, &quot;KIMBERLY KIM  KIM KIM&quot;, &quot;SKIMBOARD&quot;,
                &quot; KIM &quot;, &quot; KIM&quot;, &quot;SKIMBOARD&quot;,
            };
            for (int i = 0; i &lt; src.Length; i++)
            {
                cells[i/4, i&lt;&lt;1].PutValue(src[i]);
            }
            ReplaceOptions opts = new ReplaceOptions();
            opts.RegexKey = true;
            wb.Replace(&quot;\\bKIM\\b&quot;, &quot;^&quot;, opts);
            string[] expected = new string[]
            {
                &quot;^&quot;, &quot;rONNIE CALLED ^ AND KIMINFORMED ^  HER.&quot;, &quot;KIMBERLY ^  ^ ^&quot;, &quot;SKIMBOARD&quot;,
                &quot; ^ &quot;, &quot; ^&quot;, &quot;SKIMBOARD&quot;,
            };
            StringBuilder err = null;
            for (int i = 0; i &lt; src.Length; i++)
            {
                string v = cells[i/4, i &lt;&lt; 1].StringValue;
                if (!expected[i].Equals(v))
                {
                    if (err == null)
                    {
                        err = new StringBuilder();
                        err.Append(&quot;Regex replace:\n&quot;);
                    }
                    err.Append(&apos;[&apos;);
                    err.Append(src[i]);
                    err.Append(&quot;] should be replaced to \n[&quot;);
                    err.Append(expected[i]);
                    err.Append(&quot;] but was \n[&quot;);
                    err.Append(v);
                    err.Append(&quot;]\n&quot;);
                }
            }
            for (int i = 0; i &lt; src.Length; i++)
            {
                cells[i / 4, i &lt;&lt; 1].PutValue(src[i]);
            }
            opts.RegexKey = false;
            opts.MatchEntireCellContents = false;
            wb.Replace(&quot; KIM &quot;, &quot;^&quot;, opts);
            expected[0] = &quot;KIM&quot;;
            expected[1] = &quot;rONNIE CALLED^AND KIMINFORMED^ HER.&quot;;
            expected[2] = &quot;KIMBERLY^^KIM&quot;;
            expected[4] = &quot;^&quot;;
            expected[5] = &quot; KIM&quot;;
            if (err != null)
            {
                err.Append(&quot;\nNoRegex replace:\n&quot;);
            }
            for (int i = 0; i &lt; src.Length; i++)
            {
                string v = cells[i / 4, i &lt;&lt; 1].StringValue;
                if (!expected[i].Equals(v))
                {
                    if (err == null)
                    {
                        err = new StringBuilder();
                        err.Append(&quot;NoRegex replace:\n&quot;);
                    }
                    err.Append(&apos;[&apos;);
                    err.Append(src[i]);
                    err.Append(&quot;] should be replaced to \n[&quot;);
                    err.Append(expected[i]);
                    err.Append(&quot;] but was \n[&quot;);
                    err.Append(v);
                    err.Append(&quot;]\n&quot;);
                }
            }
            opts.CaseSensitive = false;
            src[4] = &quot; kiM &quot;;
            for (int i = 0; i &lt; src.Length; i++)
            {
                cells[i / 4, i &lt;&lt; 1].PutValue(src[i]);
            }
            if (err != null)
            {
                err.Append(&quot;\nIgnoreCase replace:\n&quot;);
            }
            wb.Replace(&quot; KIM &quot;, &quot;^&quot;, opts);
            for (int i = 0; i &lt; src.Length; i++)
            {
                string v = cells[i / 4, i &lt;&lt; 1].StringValue;
                if (!expected[i].Equals(v))
                {
                    if (err == null)
                    {
                        err = new StringBuilder();
                        err.Append(&quot;IgnoreCase replace:\n&quot;);
                    }
                    err.Append(&apos;[&apos;);
                    err.Append(src[i]);
                    err.Append(&quot;] should be replaced to \n[&quot;);
                    err.Append(expected[i]);
                    err.Append(&quot;] but was \n[&quot;);
                    err.Append(v);
                    err.Append(&quot;]\n&quot;);
                }
            }
            if (err != null)
            {
                Assert.Fail(err.ToString());
            }
        }
```

### See Also

* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


