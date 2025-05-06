---
title: StyleFlag.StyleFlag
second_title: Aspose.Cells for .NET API Reference
description: StyleFlag constructor. Constructs an object with all flags as false
type: docs
url: /net/aspose.cells/styleflag/styleflag/
---
## StyleFlag constructor

Constructs an object with all flags as false.

```csharp
public StyleFlag()
```

### Examples

```csharp
// Called: StyleFlag flag = new StyleFlag();
[Test]
        public void StyleFlag_Constructor()
        {
            //}
            Workbook workbook = new Workbook();

            // Create a designer workbook

            // Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Husband Name&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;&amp;=Husband.Name&quot;);

            worksheet.Cells[&quot;B1&quot;].PutValue(&quot;Husband Age&quot;);
            worksheet.Cells[&quot;B2&quot;].PutValue(&quot;&amp;=Husband.Age&quot;);

            worksheet.Cells[&quot;C1&quot;].PutValue(&quot;Wife&apos;s Name&quot;);
            worksheet.Cells[&quot;C2&quot;].PutValue(&quot;&amp;=Husband.Wives.Name&quot;);

            worksheet.Cells[&quot;D1&quot;].PutValue(&quot;Wife&apos;s Age&quot;);
            worksheet.Cells[&quot;D2&quot;].PutValue(&quot;&amp;=Husband.Wives.Age&quot;);

            // Apply Style to A1:D1
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(&quot;A1:D1&quot;);
            Aspose.Cells.Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            StyleFlag flag = new StyleFlag();
            flag.All = true;
            range.ApplyStyle(style, flag);

            // Initialize WorkbookDesigner object
            WorkbookDesigner designer = new WorkbookDesigner();

            // Load the template file
            designer.Workbook = workbook;

            List&lt;Husband&gt; list = new List&lt;Husband&gt;();

            // Create an object for the Husband class
            Husband h1 = new Husband(&quot;Mark John&quot;, 30);

            // Create the relevant Wife objects for the Husband object
            h1.Wives = new List&lt;Wife&gt;();
            /****************************************************/
            //COMMENT OR UN-COMMENT THIS WIVE DATA TO CHECK

            //h1.Wives.Add(new Wife(&quot;Chen Zhao&quot;, 34));
            //h1.Wives.Add(new Wife(&quot;Jamima Winfrey&quot;, 28));
            //h1.Wives.Add(new Wife(&quot;Reham Smith&quot;, 35));

            /****************************************************/
            // Create another object for the Husband class
            Husband h2 = new Husband(&quot;Masood Shankar&quot;, 40);

            // Create the relevant Wife objects for the Husband object
            h2.Wives = new List&lt;Wife&gt;();
            h2.Wives.Add(new Wife(&quot;Karishma Jathool&quot;, 36));
            h2.Wives.Add(new Wife(&quot;Angela Rose&quot;, 33));
            h2.Wives.Add(new Wife(&quot;Hina Khanna&quot;, 45));

            // Add the objects to the list
            list.Add(h1);
            list.Add(h2);
            // Specify the DataSource
            designer.SetDataSource(&quot;Husband&quot;, list);

            // Process the markers
            designer.Process();

            // Autofit columns
            worksheet.AutoFitColumns();
            designer.Workbook.Save(Constants.destPath + &quot;CellsNet46741.xlsx&quot;);
            Assert.AreEqual(workbook.Worksheets[0].Cells[&quot;C3&quot;].StringValue, &quot;Karishma Jathool&quot;);
            // Save the Excel file.
           

        }
```

### See Also

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


