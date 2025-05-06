---
title: WriteProtection.Author
second_title: Aspose.Cells for .NET API Reference
description: WriteProtection property. Gets and sets the author
type: docs
url: /net/aspose.cells/writeprotection/author/
---
## WriteProtection.Author property

Gets and sets the author.

```csharp
public string Author { get; set; }
```

### Examples

```csharp
// Called: writeProtection.Author = &amp;quot;John Doe&amp;quot;;
public static void Property_Author()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the workbook&apos;s settings
            WorkbookSettings settings = workbook.Settings;

            // Access the write protection settings
            WriteProtection writeProtection = settings.WriteProtection;

            // Set the author of the write protection
            writeProtection.Author = &quot;John Doe&quot;;

            // Set the password for write protection
            writeProtection.Password = &quot;password123&quot;;

            // Set the recommend read-only option
            writeProtection.RecommendReadOnly = true;

            // Check if the workbook is write protected
            bool isWriteProtected = writeProtection.IsWriteProtected;
            Console.WriteLine(&quot;Is Write Protected: &quot; + isWriteProtected);

            // Validate the password
            bool isValidPassword = writeProtection.ValidatePassword(&quot;password123&quot;);
            Console.WriteLine(&quot;Is Valid Password: &quot; + isValidPassword);

            // Save the workbook
            workbook.Save(&quot;WriteProtectionExample.xlsx&quot;);

            return;
        }
```

### See Also

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


