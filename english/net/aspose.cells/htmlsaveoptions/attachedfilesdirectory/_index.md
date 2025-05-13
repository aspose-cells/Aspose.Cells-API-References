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
// Called: Assert.IsTrue(File.Exists( Path.Combine(options.AttachedFilesDirectory , "sheet001.htm")));
        public void HtmlSaveOptions_Property_AttachedFilesDirectory()
        {
            DeletePath(_destFilesPath + "tmp\\Attach");
            String filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA41928/";
            Workbook wb = new Workbook(filePath + "diagramTest.xlsx");
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.AttachedFilesDirectory = "tmp\\Attach";
          
            wb.Save(_destFilesPath+ "example.html", options);
            string text = File.ReadAllText(_destFilesPath+ "example.html");            
            Assert.IsTrue(text.IndexOf("href=\"tmp/Attach/filelist.xml\"") > 0);
            Assert.IsTrue(File.Exists(_destFilesPath + "tmp\\Attach\\sheet001.htm"));
           
            options.AttachedFilesDirectory = Path.GetTempPath() + "JAVA41928";
            DeletePath(options.AttachedFilesDirectory);
            wb.Save(_destFilesPath + "example.html", options);
            text = File.ReadAllText(_destFilesPath + "example.html");
            Assert.IsTrue(text.IndexOf("href=\""+options.AttachedFilesDirectory.Replace("\\","/")+ "/filelist.xml") > 0);
            Assert.IsTrue(File.Exists( Path.Combine(options.AttachedFilesDirectory , "sheet001.htm")));
            DeletePath(_destFilesPath + "CellsJava45869");

#if !ExcludeHtml
            options.StreamProvider = new ExportStreamProvider(_destFilesPath + "CellsJava45869\\");
            wb.Save(_destFilesPath + "example.html", options);
            text = File.ReadAllText(_destFilesPath + "example.html");
            Assert.IsTrue(text.IndexOf("href=\""+_destFilesPath + "example.xml") > 0);
            Assert.IsTrue(File.Exists(_destFilesPath + "CellsJava45869\\sheet001.htm"));
#endif
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


