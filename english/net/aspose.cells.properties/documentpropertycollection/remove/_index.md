---
title: DocumentPropertyCollection.Remove
second_title: Aspose.Cells for .NET API Reference
description: DocumentPropertyCollection method. Removes a property with the specified name from the collection
type: docs
url: /net/aspose.cells.properties/documentpropertycollection/remove/
---
## DocumentPropertyCollection.Remove method

Removes a property with the specified name from the collection.

```csharp
public void Remove(string name)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The case-insensitive name of the property. |

### Examples

```csharp
// Called: workbook.Worksheets.CustomDocumentProperties.Remove(&amp;quot;_PID_HLINKS&amp;quot;);
[Test]
        // http://www.aspose.com/community/forums/thread/289649.aspx
        // Document corruption after opening Excel 2007 file with Aspose Cells 4.8.2.15 and resaving the filestream as a new file
        public void Method_String_()
        {
            Console.WriteLine(&quot;Method_String_()&quot;);
            string infn = path + @&quot;Resave/Summary_2011.1.4_2.xlsx&quot;;
            string outfn = Constants.destPath + @&quot;Summary_2011.1.4_2_out.xlsm&quot;;

           
            FileStream fstream = new FileStream(infn, FileMode.Open); /*docfile is path to xlsm file*/
            Workbook workbook = new Workbook(fstream);

            //To avoid aspose workbook corrupte file so close filestream
            fstream.Dispose();

            if (workbook.Worksheets.CustomDocumentProperties.Contains(&quot;_PID_HLINKS&quot;))
                workbook.Worksheets.CustomDocumentProperties.Remove(&quot;_PID_HLINKS&quot;);

            workbook.Save(outfn, SaveFormat.Xlsm);
        }
```

### See Also

* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


