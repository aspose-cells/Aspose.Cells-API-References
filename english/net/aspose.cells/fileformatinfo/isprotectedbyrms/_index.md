---
title: FileFormatInfo.IsProtectedByRMS
second_title: Aspose.Cells for .NET API Reference
description: FileFormatInfo property. Gets whether the file is protected by Microsoft Rights Management Server
type: docs
url: /net/aspose.cells/fileformatinfo/isprotectedbyrms/
---
## FileFormatInfo.IsProtectedByRMS property

Gets whether the file is protected by Microsoft Rights Management Server.

```csharp
public bool IsProtectedByRMS { get; }
```

### Examples

```csharp
// Called: writer.WriteLine($&amp;quot;Is Protected By RMS: {fileInfo.IsProtectedByRMS}&amp;quot;);
public static void Property_IsProtectedByRMS()
        {
            // Load a sample file to detect its format
            string filePath = &quot;sample.xlsx&quot;;
            FileFormatInfo fileInfo = FileFormatUtil.DetectFileFormat(filePath);

            // Display file format information
            Console.WriteLine(&quot;File Format Information:&quot;);
            Console.WriteLine($&quot;Is Protected By RMS: {fileInfo.IsProtectedByRMS}&quot;);
            Console.WriteLine($&quot;Is Encrypted: {fileInfo.IsEncrypted}&quot;);
            Console.WriteLine($&quot;File Format Type: {fileInfo.FileFormatType}&quot;);
            Console.WriteLine($&quot;Load Format: {fileInfo.LoadFormat}&quot;);

            // Save the information to a text file
            string outputFilePath = &quot;FileFormatInfo.txt&quot;;
            using (System.IO.StreamWriter writer = new System.IO.StreamWriter(outputFilePath))
            {
                writer.WriteLine(&quot;File Format Information:&quot;);
                writer.WriteLine($&quot;Is Protected By RMS: {fileInfo.IsProtectedByRMS}&quot;);
                writer.WriteLine($&quot;Is Encrypted: {fileInfo.IsEncrypted}&quot;);
                writer.WriteLine($&quot;File Format Type: {fileInfo.FileFormatType}&quot;);
                writer.WriteLine($&quot;Load Format: {fileInfo.LoadFormat}&quot;);
            }

            Console.WriteLine($&quot;File format information saved to {outputFilePath}&quot;);
        }
```

### See Also

* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


