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
// Called: Console.WriteLine(&amp;quot;Is Workbook Protected With Password: &amp;quot; + workbook.IsWorkbookProtectedWithPassword);
public static void Property_IsWorkbookProtectedWithPassword()
        {
            // Create a new Workbook instance
            Workbook workbook = new Workbook();

            // Access the default worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Set some properties of the workbook
            workbook.FileName = &quot;ExampleWorkbook.xlsx&quot;;
            workbook.DefaultStyle.Font.Name = &quot;Tahoma&quot;;

            // Add a new worksheet
            int newSheetIndex = workbook.Worksheets.Add();
            Worksheet newWorksheet = workbook.Worksheets[newSheetIndex];
            newWorksheet.Name = &quot;NewSheet&quot;;

            // Add some data to the new worksheet
            newWorksheet.Cells[&quot;A1&quot;].PutValue(&quot;Hello, Aspose.Cells!&quot;);

            // Set some document properties
            workbook.BuiltInDocumentProperties[&quot;Author&quot;].Value = &quot;John Smith&quot;;
            workbook.CustomDocumentProperties.Add(&quot;Checked by&quot;, &quot;Jane&quot;);

            // Save the workbook to a file
            workbook.Save(&quot;WorkbookExample.xlsx&quot;);

            // Display some properties
            Console.WriteLine(&quot;Workbook File Name: &quot; + workbook.FileName);
            Console.WriteLine(&quot;Default Font: &quot; + workbook.DefaultStyle.Font.Name);
            Console.WriteLine(&quot;Author: &quot; + workbook.BuiltInDocumentProperties[&quot;Author&quot;].Value);
            Console.WriteLine(&quot;Custom Property &apos;Checked by&apos;: &quot; + workbook.CustomDocumentProperties[&quot;Checked by&quot;].Value);

            // Check if the workbook is licensed
            Console.WriteLine(&quot;Is Licensed: &quot; + workbook.IsLicensed);

            // Check if the workbook is digitally signed
            Console.WriteLine(&quot;Is Digitally Signed: &quot; + workbook.IsDigitallySigned);

            // Check if the workbook contains macros
            Console.WriteLine(&quot;Has Macros: &quot; + workbook.HasMacro);

            // Check if the workbook has any tracked changes
            Console.WriteLine(&quot;Has Revisions: &quot; + workbook.HasRevisions);

            // Check the number of styles in the style pool
            Console.WriteLine(&quot;Number of Styles in Pool: &quot; + workbook.CountOfStylesInPool);

            // Check the theme name
            Console.WriteLine(&quot;Theme: &quot; + workbook.Theme);

            // Check if the workbook is protected with a password
            Console.WriteLine(&quot;Is Workbook Protected With Password: &quot; + workbook.IsWorkbookProtectedWithPassword);

            // Check if the workbook contains external links
            Console.WriteLine(&quot;Has External Links: &quot; + workbook.HasExernalLinks());

            // Dispose the workbook
            workbook.Dispose();
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


