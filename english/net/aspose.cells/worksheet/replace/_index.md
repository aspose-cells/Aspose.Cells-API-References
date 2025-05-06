---
title: Worksheet.Replace
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Replaces all cells text with a new string
type: docs
url: /net/aspose.cells/worksheet/replace/
---
## Worksheet.Replace method

Replaces all cells' text with a new string.

```csharp
public int Replace(string oldString, string newString)
```

| Parameter | Type | Description |
| --- | --- | --- |
| oldString | String | Old string value. |
| newString | String | New string value. |

### Examples

```csharp
// Called: sheet.Replace(finding, sReplace);
public static void Method_String_(Workbook workbook, string sFind, string sReplace)
        {
            string finding = sFind;

            foreach (Worksheet sheet in workbook.Worksheets)
            {
                sheet.Replace(finding, sReplace);

                for (int j = 0; j &lt; 3; j++)
                {

                    if (sheet.PageSetup.GetHeader(j) != null)

                        sheet.PageSetup.SetHeader(j, sheet.PageSetup.GetHeader(j).Replace(finding, sReplace));

                    if (sheet.PageSetup.GetFooter(j) != null)

                        sheet.PageSetup.SetFooter(j, sheet.PageSetup.GetFooter(j).Replace(finding, sReplace));

                }

            }

            foreach (Worksheet sheet in workbook.Worksheets)
            {

                sFind = sFind.Replace(&quot;&lt;&quot;, &quot;&amp;lt;&quot;);
                sFind = sFind.Replace(&quot;&gt;&quot;, &quot;&amp;gt;&quot;);

                foreach (Aspose.Cells.Drawing.TextBox mytextbox in sheet.TextBoxes)
                {


                    if (mytextbox.HtmlText != null)
                    {
                        if (mytextbox.HtmlText.IndexOf(sFind) &gt;= 0)
                        {
                            mytextbox.HtmlText = mytextbox.HtmlText.Replace(sFind, sReplace);
                        }
                    }
                }
            }
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


