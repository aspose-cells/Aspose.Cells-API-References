---
title: TxtLoadOptions.TreatQuotePrefixAsValue
second_title: Aspose.Cells for .NET API Reference
description: TxtLoadOptions property. Indicates whether the leading single quote sign should be taken as part of the value of one cell. Default is true. If it is false the leading single quote will be removed from corresponding cells value and QuotePrefix will be set as true for the cell
type: docs
url: /net/aspose.cells/txtloadoptions/treatquoteprefixasvalue/
---
## TxtLoadOptions.TreatQuotePrefixAsValue property

Indicates whether the leading single quote sign should be taken as part of the value of one cell. Default is true. If it is false, the leading single quote will be removed from corresponding cell's value and [`QuotePrefix`](../../style/quoteprefix/) will be set as true for the cell.

```csharp
public bool TreatQuotePrefixAsValue { get; set; }
```

### Examples

```csharp
// Called: TreatQuotePrefixAsValue = true,
public static void Property_TreatQuotePrefixAsValue()
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


