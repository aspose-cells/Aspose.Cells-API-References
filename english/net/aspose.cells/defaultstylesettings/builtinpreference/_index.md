---
title: DefaultStyleSettings.BuiltInPreference
second_title: Aspose.Cells for .NET API Reference
description: DefaultStyleSettings property. Indicates whether property for number format is preferrable when the style defines both builtin number and custom pattern. Default value is false that means by default custom pattern will be used to format values as long as it is not empty for one style
type: docs
url: /net/aspose.cells/defaultstylesettings/builtinpreference/
---
## DefaultStyleSettings.BuiltInPreference property

Indicates whether property for number format is preferrable when the style defines both built-in number and custom pattern. Default value is false, that means by default custom pattern will be used to format values as long as it is not empty for one style.

```csharp
public bool BuiltInPreference { get; set; }
```

### Remarks

When loading workbook from existing template file, maybe both built-in number and custom pattern are defined for one style. This property determine whether we should use the built-in number or the custom pattern when formatting values with the style.

### Examples

```csharp
// Called: wb.Settings.DefaultStyleSettings.BuiltInPreference = true;
[Test]
        public void Property_BuiltInPreference()
        {
            //CELLSNET-53482
            //en-CA: CELLSNET-55529
            string ptn = &quot;BuiltInFormat_&quot;;
            string[] files = Directory.GetFiles(Constants.sourcePath + &quot;Style&quot;, ptn + &quot;*.xlsx&quot;);
            if (files == null || files.Length &lt; 1)
            {
                Assert.Fail(&quot;Cannot find template files &quot; + ptn + &quot;*.xlsx&quot;);
            }
            StringBuilder sb = null;
            foreach (string path in files)
            {
                int v = path.IndexOf(ptn);
                Console.Write(&quot;FormattingTest.LocaleBuiltIn: &quot; + path.Substring(v) + &quot;...&quot;);
                if (v &lt; 0)
                {
                    Console.WriteLine(&quot;Ignored&quot;);
                    continue;
                }
                Workbook wb = new Workbook(path);
                wb.Settings.DefaultStyleSettings.BuiltInPreference = true;
                v += ptn.Length;
                bool addFile = true;
                string cn = path.Substring(v, path.Length - 5 - v).Replace(&apos;_&apos;, &apos;-&apos;);
                try
                {
                    wb.Settings.CultureInfo = new CultureInfo(cn);
                }
                catch (Exception e)
                {
                    if (sb == null)
                    {
                        sb = new StringBuilder(1024);
                    }
                    else
                    {
                        sb.Append(&apos;\n&apos;);
                    }
                    sb.Append(path);
                    sb.Append(&quot;\n  Failed to set CultureInfo: &quot;);
                    sb.Append(cn);
                    sb.Append(&quot;; &quot;);
                    Util.GetExceptoinInfo(e, sb);
                    addFile = false;
                    continue;
                }
                Cells cells = wb.Worksheets[0].Cells;
                v = cells.MaxDataRow;
                for (int i = 0; i &lt;= v; i++)
                {
                    for (int j = 0; j &lt; 6; j += 3)
                    {
                        Cell c = cells.CheckCell(i, j + 2);
                        if (c != null &amp;&amp; c.StringValue == &quot;x&quot;)
                        {
                            continue;
                        }
                        string d = cells[i, j].StringValue;
                        string s = cells[i, j + 1].StringValue;
                        if (d != s &amp;&amp; !s.StartsWith(&quot;###&quot;))
                        {
                            if (addFile)
                            {
                                if (sb == null)
                                {
                                    sb = new StringBuilder(1024);
                                }
                                else
                                {
                                    sb.Append(&apos;\n&apos;);
                                }
                                sb.Append(path);
                                addFile = false;
                            }
                            sb.Append(&quot;\n  &quot;);
                            sb.Append((char)(&apos;A&apos; + j));
                            sb.Append(i + 1);
                            sb.Append(&quot;(Style.Number=&quot;);
                            sb.Append(cells[i, 0].GetStyle(false).Number);
                            sb.Append(&quot;): expected [&quot;);
                            sb.Append(s);
                            sb.Append(&quot;] but was [&quot;);
                            sb.Append(d);
                            sb.Append(&apos;]&apos;);
                        }
                    }
                }
                Console.WriteLine(&quot;Finished&quot;);
            }
            if (sb != null)
            {
                Assert.Fail(sb.ToString());
            }
        }
```

### See Also

* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


