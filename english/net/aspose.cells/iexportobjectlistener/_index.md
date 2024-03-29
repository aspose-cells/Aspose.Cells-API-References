---
title: Interface IExportObjectListener
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.IExportObjectListener interface. Allows users to manipulate objects while exporting
type: docs
url: /net/aspose.cells/iexportobjectlistener/
---
## IExportObjectListener interface

Allows users to manipulate objects while exporting.

```csharp
public interface IExportObjectListener
```

## Methods

| Name | Description |
| --- | --- |
| [ExportObject](../../aspose.cells/iexportobjectlistener/exportobject/)(ExportObjectEvent) | Export one object. |

### Examples

The following example creates a Workbook, opens a file named designer.xls in it and makes the horizontal and vertical scroll bars invisible for the Workbook. It then replaces two string values with an Integer value and string value respectively within the spreadsheet and finally sends the updated file to the client browser.

```csharp
[C#]
    //custom implementation of IExportObjectListener
    class CustomExportObjectListener : IExportObjectListener
    {
        private int imgIdx = 0;
        public object ExportObject(ExportObjectEvent e)
        {
            Object source = e.GetSource();
            if (source is Shape)
            {
                Shape shape = (Shape)source;
                string url = null;
                switch (shape.MsoDrawingType)
                {
                    case MsoDrawingType.Picture:
                    {
                        url = SaveImage(((Picture)shape).Data, imgIdx, ((Picture)shape).ImageType);
                        break;
                     }
                }
                if (url != null)
                {
                    imgIdx++;
                }
                return url;
            }
            return null;
        }
        private string SaveImage(byte[] data, int imgIdx, ImageType format)
        {
            //here save the image to any location, then return the url(relative or absolute) that the generated html can get the image
            return "temp1/temp2.png";
        }
     }
     
        //Save html file with custom listener
        Workbook book = null; //build your workbook here
        HtmlSaveOptions saveOptions = new HtmlSaveOptions();
        saveOptions.ExportObjectListener = new CustomExportObjectListener();
        Stream stream = null; //build your stream here
        book.Save("res.html", saveOptions); //or here you can build your out put stream and save the workbook to stream

```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


