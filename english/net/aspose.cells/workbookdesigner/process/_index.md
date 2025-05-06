---
title: WorkbookDesigner.Process
second_title: Aspose.Cells for .NET API Reference
description: WorkbookDesigner method. Processes the smart markers and populates the data source values
type: docs
url: /net/aspose.cells/workbookdesigner/process/
---
## Process(Range, bool) {#process_1}

Processes the smart markers and populates the data source values.

```csharp
public void Process(Range range, bool isPreserved)
```

| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | The range to be processed |
| isPreserved | Boolean | True if the unrecognized smart marker is preserved. |

### Examples

```csharp
// Called: designer.Process(range, true);
[Test]
        public void Method_Boolean_()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSJAVA46279.xlsx&quot;);
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.LineByLine = (false);
            designer.Workbook = (wb);
            designer.SetJsonDataSource(&quot;RootData&quot;, File.ReadAllText(Constants.sourcePath + &quot;CELLSJAVA46279.json&quot;));
            Aspose.Cells.Range range = wb.Worksheets[0].Cells.CreateRange(&quot;A24:H28&quot;);
            range.Name = &quot;_CellsSmartMarkers&quot;;
            designer.Process(range, true);

            range = wb.Worksheets[0].Cells.CreateRange(&quot;A18:D19&quot;);
            range.Name = &quot;_CellsSmartMarkers&quot;;
            designer.Process(range, true);

            range = wb.Worksheets[0].Cells.CreateRange(&quot;A2:H15&quot;);
            range.Name = &quot;_CellsSmartMarkers&quot;;
            designer.Process(range, true);
            Assert.AreEqual(&quot;director last 2&quot;, wb.Worksheets[0].Cells[&quot;D38&quot;].StringValue);
            Assert.AreEqual(&quot;fff department&quot;, wb.Worksheets[0].Cells[&quot;H61&quot;].StringValue);
            wb.Save(Constants.destPath + &quot;CELLSJAVA46279.xlsx&quot;);
        }
```

### See Also

* class [Range](../../range/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Process() {#process}

Processes the smart markers and populates the data source values.

```csharp
public void Process()
```

### Examples

```csharp
// Called: template1.Process();
[Test]
        public void Method_Process()
        {
            WorkbookDesigner template1 = new WorkbookDesigner();
            template1.Workbook = new Workbook(Constants.sourcePath + &quot;SmartMarker/CellsNet48455_1.xlsx&quot;);
            WorkbookDesigner template2 = new WorkbookDesigner();
            template2.Workbook = new Workbook(Constants.sourcePath + &quot;SmartMarker/CellsNet48455_2.xlsx&quot;);

            Workbook newWorkbook = new Workbook();
            newWorkbook.Worksheets.Clear();

            // Dummy notes text
            List&lt;string&gt; ProductNotes = new List&lt;string&gt;()
            {
                &quot;ABC&quot;,
                &quot;&lt;B&gt;ABC&lt;B&gt;&quot;,
                &quot;CDE&quot;
            };
            List&lt;string&gt; TermsAndConditionsNotes = new List&lt;string&gt;()
            {
                &quot;XYZjdvskjbkj&lt;br&gt;sdfhdskjfhkj&lt;br&gt;eurfhwieufh&quot;,
                &quot;DEF&quot;,
                &quot;&lt;B&gt;AXC&lt;/B&gt;&quot;,
            };
            var data = new
            {
                CustomerOrganizationName = &quot;ABC Corp&quot;,
                QuoteNumberText = &quot;ABC&quot;,
                CreationDateText = &quot;ABC&quot;,
                EffectiveDurationText = &quot;ABC&quot;,
                EnrollmentNumberText = &quot;ABC&quot;,
                PaymentScheduleText = &quot;ABC&quot;,
                PaymentScheduleTrueUpText = &quot;ABC&quot;,
                BillingCurrencyText = &quot;ABC&quot;,
                TermOfAgreementText = &quot;ABC&quot;,
                OpportunityIDText = &quot;ABC&quot;,
                FrameworkIDText = &quot;ABC&quot;,
                CustomerContactText = &quot;ABC&quot;,
                PartnerContactsText = &quot;ABC&quot;,
                MicrosoftContactText = &quot;ABC&quot;,
                LanguageText = &quot;ABC&quot;,
                DaysText = &quot;ABC&quot;,
                PriceListMonthText = &quot;ABC&quot;,
                QuoteNumber = &quot;ABC&quot;,
                PaymentSchedule = &quot;ABC&quot;,
                PaymentScheduleTrueUp = &quot;ABC&quot;,
                BillingCurrency = &quot;ABC&quot;,
                AgreementTerm = &quot;ABC&quot;,
                OptyID = &quot;ABC&quot;,
                FrameworkID = &quot;ABC&quot;,
                EnrollmentNumber = &quot;ABC&quot;,
                CreationDate = DateTime.UtcNow,
            };

            // Bind Data
            BindData(template1, &quot;Header&quot;, new ArrayList() { data });
            BindData(template2, &quot;ProductNotes&quot;, ProductNotes.Select(note =&gt; new { NoteText = note }).ToList());
            BindData(template2, &quot;TermsAndConditions&quot;, TermsAndConditionsNotes.Select(note =&gt; new { NoteText = note }).ToList());

            // Process Data
            template1.Process();
            template2.Process();
            newWorkbook.Combine(template1.Workbook);
            newWorkbook.Combine(template2.Workbook);
                foreach (Worksheet worksheet in newWorkbook.Worksheets)
            {
                worksheet.AutoFitRows(new AutoFitterOptions
                {
                    AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                    AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph,
                    MaxRowHeight = int.MaxValue,
                    OnlyAuto = true
                });

            }
            Assert.AreEqual(48, newWorkbook.Worksheets[1].Cells.GetRowHeightPixel(8));
           
            newWorkbook.Save(Constants.destPath + &quot;CellsNet48455.xlsx&quot;);
        }
```

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Process(bool) {#process_2}

Processes the smart markers and populates the data source values.

```csharp
public void Process(bool isPreserved)
```

| Parameter | Type | Description |
| --- | --- | --- |
| isPreserved | Boolean | True if the unrecognized smart marker is preserved. |

### Examples

```csharp
// Called: designer.Process(false);
[Test]
        public void Method_Boolean_()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSJAVA45705.xlsx&quot;);
            String data = &quot;{\n&quot; + &quot;    \&quot;array\&quot;: [\n&quot; + &quot;        \&quot;English\&quot;,\n&quot; + &quot;        \&quot;Arabic\&quot;,\n&quot;
                  + &quot;        \&quot;Hindi\&quot;,\n&quot; + &quot;        \&quot;Urdu\&quot;,\n&quot; + &quot;        \&quot;French\&quot;\n&quot; + &quot;    ],\n&quot;
                  + &quot;    \&quot;var\&quot;: \&quot;This is a sentence using one place holder\&quot;,\n&quot; + &quot;\&quot;arrObj\&quot;: [\n&quot; + &quot;    {\n&quot;
                  + &quot;        \&quot;name\&quot;: \&quot;John Doe\&quot;,\n&quot; + &quot;        \&quot;age\&quot;: \&quot;27\&quot;\n&quot; + &quot;    },\n&quot; + &quot;    {\n&quot;
                  + &quot;        \&quot;name\&quot;: \&quot;Jane Doe\&quot;,\n&quot; + &quot;        \&quot;age\&quot;: \&quot;27\&quot;\n&quot; + &quot;    }\n&quot; + &quot;]&quot; + &quot;}&quot;;
          
            WorkbookDesigner designer = new WorkbookDesigner(wb);
            designer.SetJsonDataSource(&quot;ds&quot;, data);
            designer.Process(false);
            wb.Save(Constants.destPath + &quot;CELLSJAVA45705.xlsx&quot;);
            Assert.AreEqual(&quot;Arabic&quot;, wb.Worksheets[0].Cells[&quot;A9&quot;].StringValue);
            Assert.AreEqual(&quot;27&quot;, wb.Worksheets[0].Cells[&quot;B3&quot;].StringValue);

        }
```

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Process(int, bool) {#process_3}

Processes the smart markers and populates the data source values.

```csharp
public void Process(int sheetIndex, bool isPreserved)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | Int32 | Worksheet index. |
| isPreserved | Boolean | True if the unrecognized smart marker is preserved. |

### Remarks

This method works on worksheet level.

### Examples

```csharp
// Called: designer.Process(0, false);
[Test]
        public void Method_Boolean_()
        {
            List&lt;Department&gt; departments = new List&lt;Department&gt;();
            List&lt;Student&gt; students = new List&lt;Student&gt;();
            Student student1 = new Student();
            student1.EmailId = &quot;ewe@kkk.com&quot;;
            student1.Name = &quot;Jimit&quot;;
            student1.PhoneNumber = &quot;1213123213&quot;;
            Student student2 = new Student();
            student2.EmailId = &quot;ewe@kkk.com&quot;;
            student2.Name = &quot;Jimit&quot;;
            student2.PhoneNumber = &quot;1213123213&quot;;
            Student student3 = new Student();
            student3.EmailId = &quot;ewe@kkk.com&quot;;
            student3.Name = &quot;Jimit&quot;;
            student3.PhoneNumber = &quot;1213123213&quot;;
            students.Add(student1);
            students.Add(student2);
            students.Add(student3);

            Department department1 = new Department();
            department1.Name = &quot;Science&quot;;
            department1.ProfessorName = &quot;C.V&quot;;
            department1.EmailId = &quot;gh@hwe.com&quot;;
            department1.Subject = &quot;Physics&quot;;
            department1.Students = students;

            Department department2 = new Department();
            department2.Name = &quot;History&quot;;
            department2.ProfessorName = &quot;CR.V&quot;;
            department2.EmailId = &quot;wew@hwe.com&quot;;
            department2.Subject = &quot;Ancient History&quot;;
            department2.Students = students;

            departments.Add(department1);
            departments.Add(department2);
            WorkbookDesigner designer = new WorkbookDesigner();
            //WorkbookDesigner result = new WorkbookDesigner();
            designer.Workbook =
                    new Workbook(Constants.sourcePath+ &quot;SmartMarker/47888.xlsx&quot;);
            //foreach (var department in departments)
            //{
            //    MapDepartment(designer, department);
            //}
            designer.LineByLine = false;
            designer.SetDataSource(&quot;Department&quot;, departments);
            designer.Process(0, false);
            designer.Workbook.Save(Constants.destPath + &quot;47888.xlsx&quot;);
            Assert.AreEqual(&quot;History&quot;, designer.Workbook.Worksheets[0].Cells[&quot;B8&quot;].StringValue);
         
        }
```

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


