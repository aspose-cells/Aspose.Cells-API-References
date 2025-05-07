---
title: Workbook.IsWorkbookProtectedWithPassword
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Indicates whether structure or window is protected with password
type: docs
url: /net/aspose.cells/workbook/isworkbookprotectedwithpassword/
---
## Workbook.IsWorkbookProtectedWithPassword property

Indicates whether structure or window is protected with password.

```csharp
public bool IsWorkbookProtectedWithPassword { get; }
```

### Examples

```csharp
// Called: Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);
public static void Property_IsWorkbookProtectedWithPassword()
        {
            // Create a new Workbook instance
            Workbook workbook = new Workbook();

            // Access the default worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Set some properties of the workbook
            workbook.FileName = "ExampleWorkbook.xlsx";
            workbook.DefaultStyle.Font.Name = "Tahoma";

            // Add a new worksheet
            int newSheetIndex = workbook.Worksheets.Add();
            Worksheet newWorksheet = workbook.Worksheets[newSheetIndex];
            newWorksheet.Name = "NewSheet";

            // Add some data to the new worksheet
            newWorksheet.Cells["A1"].PutValue("Hello, Aspose.Cells!");

            // Set some document properties
            workbook.BuiltInDocumentProperties["Author"].Value = "John Smith";
            workbook.CustomDocumentProperties.Add("Checked by", "Jane");

            // Save the workbook to a file
            workbook.Save("WorkbookExample.xlsx");

            // Display some properties
            Console.WriteLine("Workbook File Name: " + workbook.FileName);
            Console.WriteLine("Default Font: " + workbook.DefaultStyle.Font.Name);
            Console.WriteLine("Author: " + workbook.BuiltInDocumentProperties["Author"].Value);
            Console.WriteLine("Custom Property 'Checked by': " + workbook.CustomDocumentProperties["Checked by"].Value);

            // Check if the workbook is licensed
            Console.WriteLine("Is Licensed: " + workbook.IsLicensed);

            // Check if the workbook is digitally signed
            Console.WriteLine("Is Digitally Signed: " + workbook.IsDigitallySigned);

            // Check if the workbook contains macros
            Console.WriteLine("Has Macros: " + workbook.HasMacro);

            // Check if the workbook has any tracked changes
            Console.WriteLine("Has Revisions: " + workbook.HasRevisions);

            // Check the number of styles in the style pool
            Console.WriteLine("Number of Styles in Pool: " + workbook.CountOfStylesInPool);

            // Check the theme name
            Console.WriteLine("Theme: " + workbook.Theme);

            // Check if the workbook is protected with a password
            Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);

            // Check if the workbook contains external links
            Console.WriteLine("Has External Links: " + workbook.HasExernalLinks());

            // Dispose the workbook
            workbook.Dispose();
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


