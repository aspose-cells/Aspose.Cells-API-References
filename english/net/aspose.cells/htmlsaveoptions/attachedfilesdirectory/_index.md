---
title: HtmlSaveOptions.AttachedFilesDirectory
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. The directory that the attached files will be saved to. Only for saving to html stream
type: docs
url: /net/aspose.cells/htmlsaveoptions/attachedfilesdirectory/
---
## HtmlSaveOptions.AttachedFilesDirectory property

The directory that the attached files will be saved to. Only for saving to html stream.

```csharp
public string AttachedFilesDirectory { get; set; }
```

### Examples

```csharp
// Called: saveOptions.AttachedFilesDirectory = FullPath;
private static void Property_AttachedFilesDirectory()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET49266.xlsx&quot;);//one sheet
            string destPath = _destFilesPath + &quot;CELLSNET49266.html&quot;;
            string FullPath = Path.GetFullPath(destPath);

            using (FileStream fs = File.Create(destPath))
            {
                HtmlSaveOptions saveOptions = new HtmlSaveOptions();
                saveOptions.AttachedFilesDirectory = FullPath;
                workbook.Save(fs, saveOptions);

            }
           string text =  File.ReadAllText(destPath);
            string d = &quot;src=\&quot;&quot;+ Path.GetDirectoryName(FullPath)+&quot;_files&quot;;
            Assert.IsTrue(text.IndexOf(d) != -1);


        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


