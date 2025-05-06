---
title: Chart.Name
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets and sets the name of the chart
type: docs
url: /net/aspose.cells.charts/chart/name/
---
## Chart.Name property

Gets and sets the name of the chart.

```csharp
public string Name { get; set; }
```

### Examples

```csharp
// Called: if (item.Name.Equals(&amp;quot;Sleeve1&amp;quot;, StringComparison.OrdinalIgnoreCase))
[Test]
        public void Property_Name()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet46541.xlsx&quot;);
            Worksheet worksheet = workbook.Worksheets[&quot;x&quot;];
            Chart chart = null;
            ChartCollection collection = worksheet.Charts;
            foreach (Chart item in collection)
            {
                if (item.Name.Equals(&quot;Sleeve1&quot;, StringComparison.OrdinalIgnoreCase))
                {
                    chart = item;
                    break;
                }
            }
            chart.NSeries.CategoryData = &quot;{Jan-07,Feb-07,Mar-07,Apr-07,May-07,Jun-07,Jul-07,Aug-07,Sep-07,Oct-07,Nov-07,Dec-07,Jan-08,Feb-08,Mar-08,Apr-08,May-08,Jun-08,Jul-08,Aug-08,Sep-08,Oct-08,Nov-08,Dec-08,Jan-09,Feb-09,Mar-09,Apr-09,May-09,Jun-09,Jul-09,Aug-09,Sep-09,Oct-09,Nov-09,Dec-09,Jan-10,Feb-10,Mar-10,Apr-10,May-10,Jun-10,Jul-10,Aug-10,Sep-10,Oct-10,Nov-10,Dec-10,Jan-11,Feb-11,Mar-11,Apr-11,May-11,Jun-11,Jul-11,Aug-11,Sep-11,Oct-11,Nov-11,Dec-11,Jan-12,Feb-12,Mar-12,Apr-12,May-12,Jun-12,Jul-12,Aug-12,Sep-12,Oct-12,Nov-12,Dec-12,Jan-13,Feb-13,Mar-13,Apr-13,May-13,Jun-13,Jul-13,Aug-13,Sep-13,Oct-13,Nov-13,Dec-13,Jan-14,Feb-14,Mar-14,Apr-14,May-14,Jun-14,Jul-14,Aug-14,Sep-14,Oct-14,Nov-14,Dec-14,Jan-15,Feb-15,Mar-15,Apr-15,May-15,Jun-15,Jul-15,Aug-15,Sep-15,Oct-15,Nov-15,Dec-15,Jan-16,Feb-16,Mar-16,Apr-16,May-16,Jun-16,Jul-16,Aug-16,Sep-16,Oct-16,Nov-16,Dec-16,Jan-17,Feb-17,Mar-17,Apr-17,May-17,Jun-17,Jul-17,Aug-17,Sep-17,Oct-17,Nov-17,Dec-17,Jan-18,Feb-18,Mar-18,Apr-18,May-18,Jun-18,Jul-18,Aug-18,Sep-18,Oct-18,Nov-18,Dec-18}&quot;;
            Series series = chart.NSeries[0];

            series.Values = &quot;{#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,1.093,1.082,0.9348,1.009,0.904,0.8071,0.6833,0.6315,0.5006,0.4844,0.5873,0.545,0.5408,0.5686,0.6371,0.6219,0.6211,0.5992,0.7537,0.6912,0.7974,0.8143,0.7866,0.7713,0.7702,0.7917,0.7639,0.7233,0.7549,0.7643,0.6235,0.5935,0.6282,0.5988,0.6388,0.7434,0.8174,0.7898,0.9979,1.236,1.399,1.534,1.518,1.576,1.498,1.526,1.411,1.347,1.354,1.646,1.528,1.361,1.237,1.109,1.128,1.218,1.342,1.463,1.57,1.628,1.674,1.294,1.246,1.107,1.055,1.084,0.9775,0.819,0.6664,0.7173,0.6019,0.5725,0.56,0.6035,0.5761,0.5943,0.5834,0.5283,0.6451,0.7256,0.7424}&quot;;
            series.XValues = chart.NSeries.CategoryData;
            series = chart.NSeries[1];
            series.Values = &quot;{#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,#N/A,0.8502,1.143,1.015,1.451,1.456,1.546,1.339,0.9836,0.6883,0.785,0.73,0.4982,0.3184,0.3848,0.4471,0.2221,0.4049,0.3442,0.5985,0.8323,0.9023,0.977,0.6374,0.8251,0.5274,0.5676,0.2838,0.6943,0.6724,1.094,0.8936,1.17,0.7592,0.774,0.6699,0.8001,0.4543,0.0532,0.1368,0.0796,0.1161,0.5887,0.6462,1.3345,1.3193,1.4851,1.0831,1.576,2.1996,2.5776,2.328,1.69,1.2115,0.6938,0.5675,0.5772,0.6006,0.5947,1.9482,2.4148,2.7045,1.266,0.8576,0.8601,1.1484,1.616,1.8641,1.917,1.5983,1.0934,0.5781,0.6311,0.494,0.4923,0.4531,0.5922,0.4059,0.157,0.5382,0.7509,0.7378,0.2127,0.4207,0.6209,0.6202,0.4217,0.4677,0.2873,0.3347,0.3535}&quot;;
            series.XValues = chart.NSeries.CategoryData;

            workbook.Save(Constants.destPath + &quot;CellsNet46541.xlsx&quot;);
        }
```

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


