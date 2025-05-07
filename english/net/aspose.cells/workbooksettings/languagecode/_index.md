---
title: WorkbookSettings.LanguageCode
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file
type: docs
url: /net/aspose.cells/workbooksettings/languagecode/
---
## WorkbookSettings.LanguageCode property

Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file.

```csharp
public CountryCode LanguageCode { get; set; }
```

### Examples

```csharp
// Called: workbook.Settings.LanguageCode = CountryCode.USA;
public static void Property_LanguageCode()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Set the country code for the workbook
            workbook.Settings.LanguageCode = CountryCode.USA;
            workbook.Settings.Region = CountryCode.USA;

            // Add some data to the worksheet
            worksheet.Cells[0, 0].PutValue("Country");
            worksheet.Cells[0, 1].PutValue("Code");

            worksheet.Cells[1, 0].PutValue("United States");
            worksheet.Cells[1, 1].PutValue((int)CountryCode.USA);

            worksheet.Cells[2, 0].PutValue("Canada");
            worksheet.Cells[2, 1].PutValue((int)CountryCode.Canada);

            worksheet.Cells[3, 0].PutValue("France");
            worksheet.Cells[3, 1].PutValue((int)CountryCode.France);

            worksheet.Cells[4, 0].PutValue("Germany");
            worksheet.Cells[4, 1].PutValue((int)CountryCode.Germany);

            // Save the workbook
            workbook.Save("CountryCodeExample.xlsx");
            workbook.Save("CountryCodeExample.pdf");
            return;
        }
```

### See Also

* enum [CountryCode](../../countrycode/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


