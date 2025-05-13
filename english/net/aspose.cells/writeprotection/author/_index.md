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
// Called: writeProtection.Author = "John Doe";
public static void WriteProtection_Property_Author()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the workbook's settings
            WorkbookSettings settings = workbook.Settings;

            // Access the write protection settings
            WriteProtection writeProtection = settings.WriteProtection;

            // Set the author of the write protection
            writeProtection.Author = "John Doe";

            // Set the password for write protection
            writeProtection.Password = "password123";

            // Set the recommend read-only option
            writeProtection.RecommendReadOnly = true;

            // Check if the workbook is write protected
            bool isWriteProtected = writeProtection.IsWriteProtected;
            Console.WriteLine("Is Write Protected: " + isWriteProtected);

            // Validate the password
            bool isValidPassword = writeProtection.ValidatePassword("password123");
            Console.WriteLine("Is Valid Password: " + isValidPassword);

            // Save the workbook
            workbook.Save("WriteProtectionExample.xlsx");

            return;
        }
```

### See Also

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


