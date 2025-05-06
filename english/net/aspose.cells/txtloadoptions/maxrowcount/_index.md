---
title: TxtLoadOptions.MaxRowCount
second_title: Aspose.Cells for .NET API Reference
description: TxtLoadOptions property. The maximum count of rows to be imported for one sheet
type: docs
url: /net/aspose.cells/txtloadoptions/maxrowcount/
---
## TxtLoadOptions.MaxRowCount property

The maximum count of rows to be imported for one sheet.

```csharp
public int MaxRowCount { get; set; }
```

### Remarks

Those rows exceeding this limit will be ignored or extended to next sheet according to [`ExtendToNextSheet`](../extendtonextsheet/). This count includes the header rows([`HeaderRowsCount`](../headerrowscount/)). The maximum allowed value of it is the row limit of corresponding file format, such as for xlsx file it 1048576. If this property has not been specified or the specified value is not positive, then the maximum limit will be used too.

### Examples

```csharp
// Called: MaxRowCount = 1000,
public static void Property_MaxRowCount()
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


