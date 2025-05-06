---
title: PageSetup.GetHeader
second_title: Aspose.Cells for .NET API Reference
description: PageSetup method. Gets a script formatting the header of an Excel file
type: docs
url: /net/aspose.cells/pagesetup/getheader/
---
## PageSetup.GetHeader method

Gets a script formatting the header of an Excel file.

```csharp
public string GetHeader(int section)
```

| Parameter | Type | Description |
| --- | --- | --- |
| section | Int32 | 0: Left Section, 1: Center Section, 2: Right Section. |

### Examples

```csharp
// Called: + odsSetup.GetHeader(1) + &amp;quot;:&amp;quot; + odsSetup.GetHeader(2));
public void Method_Int32_(string dir, StreamWriter writer)
        {
            if (Directory.Exists(dir))
            {
                string[] infns = Directory.GetFileSystemEntries(dir);
                for (int i = 0; i &lt; infns.Length; i++)
                {
                    string infn = infns[i];
                    if (File.Exists(infn) &amp;&amp; infn.Split(&apos;.&apos;)[1] != &quot;ods&quot;)
                    {
                        try
                        {
                            Console.WriteLine(&quot;Processing file: &quot; + infn);
                            writer.WriteLine(&quot;Input file: &quot; + infn);
                            Workbook workbook = new Workbook(infn);

                            PageSetup xlsSetup = workbook.Worksheets[0].PageSetup;

                            string[] splitInfn = infn.Split(&apos;.&apos;);
                            string outfn = splitInfn[0] + &quot;_in.ods&quot;;
                            writer.WriteLine(&quot;Output ODS file: &quot; + outfn);
                            workbook.Save(outfn, SaveFormat.Ods);

                            workbook = new Workbook(outfn);

                            PageSetup odsSetup = workbook.Worksheets[0].PageSetup;

                            outfn = splitInfn[0] + &quot;_out.ods&quot;;
                            writer.WriteLine(&quot;Processed ODS file: &quot; + outfn);
                            workbook.Save(outfn, SaveFormat.Ods);

                            writer.WriteLine(&quot;XLS Header: &quot; + xlsSetup.GetHeader(0) + &quot;:&quot;
                                + xlsSetup.GetHeader(1) + &quot;:&quot; + xlsSetup.GetHeader(2));
                            writer.WriteLine(&quot;ODS Header: &quot; + odsSetup.GetHeader(0) + &quot;:&quot;
                                + odsSetup.GetHeader(1) + &quot;:&quot; + odsSetup.GetHeader(2));
                            writer.WriteLine(&quot;XLS Footer: &quot; + xlsSetup.GetFooter(0) + &quot;:&quot;
                                + xlsSetup.GetFooter(1) + &quot;:&quot; + xlsSetup.GetFooter(2));
                            writer.WriteLine(&quot;ODS Footer: &quot; + odsSetup.GetFooter(0) + &quot;:&quot;
                                + odsSetup.GetFooter(1) + &quot;:&quot; + odsSetup.GetFooter(2));
                        }
                        catch (Exception e)
                        {
                            Console.WriteLine(&quot;Processed error file: &quot; + infn);
                            writer.WriteLine(e.StackTrace);
                        }
                    }
                    else
                    {
                        Method_Int32_(infn, writer);
                    }
                }
            }
        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


