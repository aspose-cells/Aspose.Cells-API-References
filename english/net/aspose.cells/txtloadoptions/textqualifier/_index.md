---
title: TxtLoadOptions.TextQualifier
second_title: Aspose.Cells for .NET API Reference
description: TxtLoadOptions property. Specifies the text qualifier for cell values. Default qualifier is 
type: docs
url: /net/aspose.cells/txtloadoptions/textqualifier/
---
## TxtLoadOptions.TextQualifier property

Specifies the text qualifier for cell values. Default qualifier is '"'.

```csharp
public char TextQualifier { get; set; }
```

### Remarks

When setting this property, [`HasTextQualifier`](../hastextqualifier/) will become true automatically.

### Examples

```csharp
// Called: TextQualifier = &amp;apos;\&amp;quot;&amp;apos;,
public static void Property_TextQualifier()
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


