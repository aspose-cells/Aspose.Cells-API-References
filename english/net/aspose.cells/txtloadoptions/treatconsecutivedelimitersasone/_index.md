---
title: TxtLoadOptions.TreatConsecutiveDelimitersAsOne
second_title: Aspose.Cells for .NET API Reference
description: TxtLoadOptions property. Whether consecutive delimiters should be treated as one
type: docs
url: /net/aspose.cells/txtloadoptions/treatconsecutivedelimitersasone/
---
## TxtLoadOptions.TreatConsecutiveDelimitersAsOne property

Whether consecutive delimiters should be treated as one.

```csharp
public bool TreatConsecutiveDelimitersAsOne { get; set; }
```

### Examples

```csharp
// Called: tlo.TreatConsecutiveDelimitersAsOne = true;
[Test]
        public void Property_TreatConsecutiveDelimitersAsOne()
        {
            TxtLoadOptions tlo = new TxtLoadOptions(LoadFormat.Csv);
            Workbook wb = LoadAsCsv(&quot;1,\&quot;abc\&quot;,3,&apos;def&apos;\n\&quot;\&quot;\&quot;g&apos;hi\&quot;,,,\n&apos;jkl\&quot;&apos;,,,12&quot;, tlo);
            Cells cells = wb.Worksheets[0].Cells;
            Assert.AreEqual(&quot;abc&quot;, cells[&quot;B1&quot;].Value, &quot;Default-B1.Value&quot;);
            Assert.AreEqual(&quot;&apos;def&apos;&quot;, cells[&quot;D1&quot;].Value, &quot;Default-D1.Value&quot;);
            Assert.AreEqual(&quot;\&quot;g&apos;hi&quot;, cells[&quot;A2&quot;].Value, &quot;Default-A2.Value&quot;);
            Assert.AreEqual(&quot;&apos;jkl\&quot;&apos;&quot;, cells[&quot;A3&quot;].Value, &quot;Default-D2.Value&quot;);
            Assert.AreEqual(CellValueType.IsNull, cells[&quot;B3&quot;].Type, &quot;Default-B3.Type&quot;);
            Assert.AreEqual(12, cells[&quot;D3&quot;].IntValue, &quot;Default-D3.IntValue&quot;);

            tlo.TreatConsecutiveDelimitersAsOne = true;
            wb = LoadAsCsv(&quot;1,\&quot;abc\&quot;,3,&apos;def&apos;\n\&quot;\&quot;\&quot;g&apos;hi\&quot;,,,\n&apos;jkl\&quot;&apos;,,,12&quot;, tlo);
            cells = wb.Worksheets[0].Cells;
            Assert.AreEqual(CellValueType.IsNull, cells[&quot;D3&quot;].Type, &quot;ConsecutiveDelimitersAsOne-D3.Type&quot;);
            Assert.AreEqual(12, cells[&quot;B3&quot;].IntValue, &quot;ConsecutiveDelimitersAsOne-B3.IntValue&quot;);

            /*tlo.TreatConsecutiveDelimitersAsOne = true;
            tlo.TextQualifier = &apos;\&apos;&apos;;
            ms.Position = 0;
            wb = new Workbook(ms, tlo);
            cells = wb.Worksheets[0].Cells;
            Assert.AreEqual(&quot;\&quot;abc\&quot;&quot;, cells[&quot;B1&quot;].Value, &quot;ConsecutiveDelimitersAsOne&amp;TextQualifier=\&quot;&apos;\&quot;-B1.Value&quot;);
            Assert.AreEqual(&quot;def&quot;, cells[&quot;D1&quot;].Value, &quot;ConsecutiveDelimitersAsOne&amp;TextQualifier=\&quot;&apos;\&quot;-D1.Value&quot;);
            Assert.AreEqual(&quot;\&quot;\&quot;\&quot;g&apos;hi\&quot;&quot;, cells[&quot;A2&quot;].Value, &quot;ConsecutiveDelimitersAsOne&amp;TextQualifier=\&quot;&apos;\&quot;-A2.Value&quot;);
            Assert.AreEqual(&quot;jkl\&quot;&quot;, cells[&quot;A3&quot;].Value, &quot;ConsecutiveDelimitersAsOne&amp;TextQualifier=\&quot;&apos;\&quot;-D2.Value&quot;);
            Assert.AreEqual(CellValueType.IsNull, cells[&quot;D3&quot;].Type, &quot;ConsecutiveDelimitersAsOne&amp;TextQualifier=\&quot;&apos;\&quot;-D3.Type&quot;);
            Assert.AreEqual(12, cells[&quot;B3&quot;].IntValue, &quot;ConsecutiveDelimitersAsOne&amp;TextQualifier=\&quot;&apos;\&quot;-B3.IntValue&quot;);*/

            tlo = new TxtLoadOptions(LoadFormat.Csv);
            tlo.Encoding = Encoding.Unicode;
            tlo.Separator = &apos; &apos;;
            wb = LoadAsCsv(&quot;1 \&quot;abc\&quot; 3 &apos;def&apos;\n\&quot;\&quot;\&quot;g&apos;hi\&quot;   \n&apos;jkl\&quot;&apos;   12&quot;, tlo);
            cells = wb.Worksheets[0].Cells;
            Assert.AreEqual(&quot;abc&quot;, cells[&quot;B1&quot;].Value, &quot;Separator=&apos; &apos;-B1.Value&quot;);
            Assert.AreEqual(&quot;&apos;def&apos;&quot;, cells[&quot;D1&quot;].Value, &quot;Separator=&apos; &apos;-D1.Value&quot;);
            Assert.AreEqual(&quot;\&quot;g&apos;hi&quot;, cells[&quot;A2&quot;].Value, &quot;Separator=&apos; &apos;-A2.Value&quot;);
            Assert.AreEqual(&quot;&apos;jkl\&quot;&apos;&quot;, cells[&quot;A3&quot;].Value, &quot;Separator=&apos; &apos;-D2.Value&quot;);
            Assert.AreEqual(CellValueType.IsNull, cells[&quot;D3&quot;].Type, &quot;Separator=&apos; &apos;-D3.Type&quot;);
            Assert.AreEqual(12, cells[&quot;B3&quot;].IntValue, &quot;Separator=&apos; &apos;-B3.IntValue&quot;);

            tlo.TreatConsecutiveDelimitersAsOne = false;
            wb = LoadAsCsv(&quot;1 \&quot;abc\&quot; 3 &apos;def&apos;\n\&quot;\&quot;\&quot;g&apos;hi\&quot;   \n&apos;jkl\&quot;&apos;   12&quot;, tlo);
            cells = wb.Worksheets[0].Cells;
            Assert.AreEqual(CellValueType.IsNull, cells[&quot;B3&quot;].Type, &quot;ConsecutiveDelimitersAsOne=false&amp;Separator=&apos; &apos;-B3.Type&quot;);
            Assert.AreEqual(12, cells[&quot;D3&quot;].IntValue, &quot;ConsecutiveDelimitersAsOne=false&amp;Separator=&apos; &apos;-D3.IntValue&quot;);

            tlo = new TxtLoadOptions(LoadFormat.Csv);
            wb = LoadAsCsv(&quot;1,\&quot;abc\n 3 &apos;def&apos;\n\&quot;\&quot;ghi&quot;, tlo);
            cells = wb.Worksheets[0].Cells;
            Assert.AreEqual(&quot;abc\n 3 &apos;def&apos;\n\&quot;ghi&quot;, cells[&quot;B1&quot;].Value, &quot;Value with multiple lines&quot;);
        }
```

### See Also

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


