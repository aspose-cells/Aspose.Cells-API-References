---
title: DocumentPropertyCollection.Contains
second_title: Aspose.Cells for .NET API Reference
description: DocumentPropertyCollection method. Returns true if a property with the specified name exists in the collection
type: docs
url: /net/aspose.cells.properties/documentpropertycollection/contains/
---
## DocumentPropertyCollection.Contains method

Returns true if a property with the specified name exists in the collection.

```csharp
public bool Contains(string name)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The case-insensitive name of the property. |

### Return Value

True if the property exists in the collection; false otherwise.

### Examples

```csharp
// Called: if (workbook.Worksheets.CustomDocumentProperties.Contains("_PID_HLINKS"))
[Test]
        // http://www.aspose.com/community/forums/thread/289649.aspx
        // Document corruption after opening Excel 2007 file with Aspose Cells 4.8.2.15 and resaving the filestream as a new file
        public void Method_String_()
        {
            Console.WriteLine("Method_String_()");
            string infn = path + @"Resave/Summary_2011.1.4_2.xlsx";
            string outfn = Constants.destPath + @"Summary_2011.1.4_2_out.xlsm";

           
            FileStream fstream = new FileStream(infn, FileMode.Open); /*docfile is path to xlsm file*/
            Workbook workbook = new Workbook(fstream);

            //To avoid aspose workbook corrupte file so close filestream
            fstream.Dispose();

            if (workbook.Worksheets.CustomDocumentProperties.Contains("_PID_HLINKS"))
                workbook.Worksheets.CustomDocumentProperties.Remove("_PID_HLINKS");

            workbook.Save(outfn, SaveFormat.Xlsm);
        }
```

### See Also

* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


