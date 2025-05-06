---
title: TxtLoadOptions.HasTextQualifier
second_title: Aspose.Cells for .NET API Reference
description: TxtLoadOptions property. Whether there is text qualifier for cell value. Default is true
type: docs
url: /net/aspose.cells/txtloadoptions/hastextqualifier/
---
## TxtLoadOptions.HasTextQualifier property

Whether there is text qualifier for cell value. Default is true.

```csharp
public bool HasTextQualifier { get; set; }
```

### Examples

```csharp
// Called: HasTextQualifier = true,
public static void Property_HasTextQualifier()
        {
            // Create an instance of TxtLoadOptions
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                Separator = &apos;,&apos;,
                SeparatorString = &quot;,&quot;,
                IsMultiEncoded = false,
                HasFormula = true,
                HasTextQualifier = true,
                TextQualifier = &apos;\&quot;&apos;,
                TreatConsecutiveDelimitersAsOne = true,
                TreatQuotePrefixAsValue = true,
                ExtendToNextSheet = false,
                HeaderRowsCount = 1,
                HeaderColumnsCount = 1,
                MaxRowCount = 1000,
                MaxColumnCount = 50,
                Encoding = Encoding.UTF8,
                LoadStyleStrategy = TxtLoadStyleStrategy.BuiltIn,
                ConvertNumericData = true,
                ConvertDateTimeData = true,
                KeepPrecision = true,
                Password = &quot;password&quot;,
                ParsingFormulaOnOpen = true,
                ParsingPivotCachedRecords = true,
                LanguageCode = CountryCode.USA,
                Region = CountryCode.USA,
                CultureInfo = new System.Globalization.CultureInfo(&quot;en-US&quot;),
                StandardFont = &quot;Arial&quot;,
                StandardFontSize = 10.5,
                InterruptMonitor = new InterruptMonitor(),
                IgnoreNotPrinted = true,
                CheckDataValid = true,
                CheckExcelRestriction = true,
                KeepUnparsedData = true,
                LoadFilter = new LoadFilter(LoadDataFilterOptions.All),
                LightCellsDataHandler = new LightCellsDataHandler(),
                MemorySetting = MemorySetting.MemoryPreference,
                WarningCallback = new WarningCallback(),
                AutoFitterOptions = new AutoFitterOptions(),
                AutoFilter = true,
                FontConfigs = new IndividualFontConfigs(),
                IgnoreUselessShapes = true,
                PreservePaddingSpacesInFormula = true
            };

            // Load a CSV file with the specified options
            Workbook workbook = new Workbook(&quot;TxtLoadOptionsExample_original.csv&quot;, loadOptions);

            // Save the workbook to an Excel file
            workbook.Save(&quot;TxtLoadOptionsExample.xlsx&quot;);

            return;
        }
```

### See Also

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


