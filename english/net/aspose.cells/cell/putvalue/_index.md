---
title: Cell.PutValue
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Puts a boolean value into the cell
type: docs
url: /net/aspose.cells/cell/putvalue/
---
## PutValue(bool) {#putvalue}

Puts a boolean value into the cell.

```csharp
public void PutValue(bool boolValue)
```

| Parameter | Type | Description |
| --- | --- | --- |
| boolValue | Boolean |  |

### Examples

```csharp
// Called: cells[r++, 0].PutValue(true);
[Test]
        public void Method_Boolean_()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            FormatConditionCollection fcc = cfc[cfc.Add()];
            fcc.AddArea(CellArea.CreateCellArea(0, 0, 30, 0));
            fcc.AddCondition(FormatConditionType.DuplicateValues);
            FormatCondition fc = fcc[0];
            fc.Style.Pattern = BackgroundType.Solid;
            fc.Style.BackgroundColor = Color.Red;
            Cells cells = sheet.Cells;
            foreach (string s in new string[] {
                &quot;true&quot;, &quot;false&quot;, &quot;#DIV/0!&quot;, &quot;#VALUE!&quot;, &quot;#N/A&quot;, &quot;#NAME?&quot;, &quot;#NUM!&quot;, &quot;#NULL!&quot;, &quot;#REF!&quot; })
            {
                cells[1, 0].Formula = &quot;=\&quot;&quot; + s + &quot;\&quot;&quot;;
                cells[2, 0].Formula = &quot;=\&quot;&quot; + s[0] + char.ToUpper(s[1]) + s.Substring(2) + &quot;\&quot;&quot;;
                object v;
                if (s[0] == &apos;t&apos;)
                {
                    v = true;
                }
                else if (s[0] == &apos;f&apos;)
                {
                    v = false;
                }
                else
                {
                    v = s;
                }
                cells[3, 0].PutValue(v);
                wb.CalculateFormula();
                for (int i = 1; i &lt; 4; i++)
                {
                    Assert.AreEqual(BackgroundType.None, cells[i, 0].GetDisplayStyle().Pattern, &quot;A&quot; + (i + 1));
                }
                cells[4, 0].PutValue(v);
                for (int i = 1; i &lt; 5; i++)
                {
                    Assert.AreEqual(BackgroundType.Solid, cells[i, 0].GetDisplayStyle().Pattern, &quot;A&quot; + (i + 1));
                }
            }

            int r = 1;
            cells[r++, 0].PutValue(true);
            cells[r++, 0].PutValue(&quot;abc&quot;);
            cells[r++, 0].PutValue(&quot;a*c&quot;);
            cells[r++, 0].PutValue(&quot;adc&quot;);
            cells[r++, 0].PutValue(&quot;&quot;);
            cells[r++, 0].PutValue(false);
            cells[r++, 0].PutValue(&quot;#NUM!&quot;);
            cells[r++, 0].PutValue(&quot;abd&quot;);
            cells[r++, 0].PutValue(true);
            cells[r++, 0].PutValue(&quot;#VALUE!&quot;);
            cells[r++, 0].PutValue(&quot;a?d&quot;);
            cells[r++, 0].PutValue(&quot;aed&quot;);
            cells[r++, 0].PutValue(&quot;#NUM!&quot;);
            cells[r++, 0].PutValue(0);
            cells[r++, 0].PutValue(&quot;2&quot;);
            cells[r++, 0].PutValue(1);
            int allMatch = r;
            cells[r++, 0].PutValue(2);
            cells[r++, 0].Formula = &quot;=\&quot;3.0\&quot;&quot;;
            cells[r++, 0].PutValue(3);
            cells[r++, 0].Formula = &quot;=\&quot;4.0\&quot;&quot;;
            cells[r++, 0].Formula = &quot;=\&quot;4\&quot;&quot;;
            cells[r++, 0].Formula = &quot;=\&quot;.3\&quot;&quot;;
            cells[r++, 0].PutValue(0.3);
            cells[r++, 0].Formula = &quot;=\&quot;3,000\&quot;&quot;;
            cells[r++, 0].PutValue(3000);
            wb.CalculateFormula();
            for (r--; r &gt; -1; r--)
            {
                Assert.AreEqual(r &lt; allMatch &amp;&amp; r % 2 == 0 ? BackgroundType.None : BackgroundType.Solid,
                    cells[r, 0].GetDisplayStyle().Pattern, &quot;A&quot; + (r + 1));
            }
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(int) {#putvalue_2}

Puts an integer value into the cell.

```csharp
public void PutValue(int intValue)
```

| Parameter | Type | Description |
| --- | --- | --- |
| intValue | Int32 | Input value |

### Examples

```csharp
// Called: cells[1, 1].PutValue(2);
[Test]
    public void Method_Int32_()
    {
      Workbook workbook = new Workbook();
      Cells cells = workbook.Worksheets[0].Cells;
      cells[0, 0].PutValue(&quot;Apple&quot;);
      cells[1, 0].PutValue(&quot;Banana&quot;);
      cells[2, 0].PutValue(&quot;Orange&quot;);
      cells[0, 1].PutValue(1);
      cells[1, 1].PutValue(2);
      cells[2, 1].PutValue(3);
      cells[0, 2].Formula = &quot;=SUMIF(A1:A3,\&quot;Banana\&quot;,B1:B3)&quot;;
      Console.WriteLine(&quot;=SUMIF(A1:A3,\&quot;Banana\&quot;,B1:B3)&quot;);
      workbook.CalculateFormula();
      Assert.AreEqual(2, cells[0, 2].IntValue);
    }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(double) {#putvalue_1}

Puts a double value into the cell.

```csharp
public void PutValue(double doubleValue)
```

| Parameter | Type | Description |
| --- | --- | --- |
| doubleValue | Double | Input value |

### Examples

```csharp
// Called: cells[2, 1].PutValue(0.69);
[Test]
        public void Method_Double_()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells[0, 0].PutValue(&quot;Fruit&quot;);
            cells[0, 1].PutValue(&quot;Price&quot;);
            cells[0, 2].PutValue(&quot;Count&quot;);
            cells[1, 0].PutValue(&quot;Apples&quot;);
            cells[1, 1].PutValue(0.69);
            cells[1, 2].PutValue(40);
            cells[2, 0].PutValue(&quot;Bananas&quot;);
            cells[2, 1].PutValue(0.69);
            cells[2, 2].PutValue(38);
            cells[3, 0].PutValue(&quot;Lemons&quot;);
            cells[3, 1].PutValue(0.55);
            cells[3, 2].PutValue(15);
            cells[4, 0].PutValue(&quot;Oranges&quot;);
            cells[4, 1].PutValue(0.25);
            cells[4, 2].PutValue(25);
            Cell cell = cells[0, 3];
            cell.Formula = &quot;=INDEX(A2:C5,1,3)&quot;;
            workbook.CalculateFormula();
            Assert.AreEqual(40, cell.IntValue);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(string, bool, bool) {#putvalue_7}

Puts a value into the cell, if appropriate the value will be converted to other data type and cell's number format will be reset.

```csharp
public void PutValue(string stringValue, bool isConverted, bool setStyle)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | String | Input value |
| isConverted | Boolean | True: converted to other data type if appropriate. |
| setStyle | Boolean | True: set the number format to cell's style when converting to other data type |

### Examples

```csharp
// Called: cells[&amp;quot;A1&amp;quot;].PutValue(&amp;quot;12:40&amp;quot;, true, true);
[Test]
        public void Method_Boolean_()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells[&quot;A1&quot;].PutValue(&quot;12:40&quot;, true, true);
            Assert.AreEqual(cells[&quot;A1&quot;].GetStyle().IsDateTime, true);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(string, bool) {#putvalue_6}

Puts a string value into the cell and converts the value to other data type if appropriate.

```csharp
public void PutValue(string stringValue, bool isConverted)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | String | Input value |
| isConverted | Boolean | True: converted to other data type if appropriate. |

### Examples

```csharp
// Called: cell.PutValue(&amp;quot;1 234&amp;quot;, true);
[Test]
        public void Method_Boolean_()
        { //Fraction numeric values
            CultureInfo ci = new CultureInfo(CultureInfo.CurrentCulture.LCID);
            ci.NumberFormat.NumberGroupSeparator = &quot; &quot;;
            Workbook wb = LoadAsCsv(&quot;1 23/50,123 23/32,1 0/123,1 234 46/125,1 234 121/125&quot;,
                new TxtLoadOptions() { CultureInfo = ci });
            Cells cells = wb.Worksheets[0].Cells;
            Cell cell;
            double[] vals = new double[] { 1.46, 123.71875, 1.0, 1234.368, 1234.968};
            for (int i = 0; i &lt; vals.Length; i++)
            {
                cell = cells[0, i];
                if(cell.NumberCategoryType != NumberCategoryType.Fraction)
                {
                    Assert.Fail(((char)(&apos;A&apos; + i)) + &quot;1: should be fraction but was &quot; + cell.NumberCategoryType);
                }
                else
                {
                    Assert.AreEqual(vals[i], cell.DoubleValue, 1.0E-6, ((char)(&apos;A&apos; + i)) + &quot;1&quot;);
                }
            }
            cell = cells[0, vals.Length];
            cell.PutValue(&quot;1 234&quot;, true);
            FormulaCaseUtil.AssertInt(1234, cell.Value, &quot;For \&quot;1 234\&quot; and space as group separator&quot;);
            wb.Settings.CultureInfo = CultureInfo.CurrentCulture;
            cell.PutValue(&quot;1 234&quot;, true);
            Assert.AreEqual(CellValueType.IsString, cell.Type, &quot;For \&quot;1 234\&quot; with default separators&quot;);
            cell.PutValue(&quot;+30 2310469658&quot;, true);
            Assert.AreEqual(CellValueType.IsString, cell.Type, &quot;For \&quot;1 234\&quot; with default separators&quot;);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(string) {#putvalue_5}

Puts a string value into the cell.

```csharp
public void PutValue(string stringValue)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | String | Input value |

### Examples

```csharp
// Called: cells[3, 1].PutValue(&amp;quot;No&amp;quot;);
[Test]
             public void Method_String_()
             {
               Workbook workbook = new Workbook();
               Cells cells = workbook.Worksheets[0].Cells;
               cells[0, 0].PutValue(&quot;apples&quot;);
               cells[2, 0].PutValue(&quot;oranges&quot;);
               cells[3, 0].PutValue(&quot;peaches&quot;);
               cells[5, 0].PutValue(&quot;apples&quot;);
               cells[0, 1].PutValue(&quot;Yes&quot;);
               cells[2, 1].PutValue(&quot;NO&quot;);
               cells[3, 1].PutValue(&quot;No&quot;);
               cells[4, 1].PutValue(&quot;YeS&quot;);
               cells[0, 2].Formula = &quot;=COUNTIF(B1:B6,\&quot;yes\&quot;)&quot;;
               Console.WriteLine(&quot;=COUNTIF(B1:B6,\&quot;yes\&quot;)&quot;);
               workbook.CalculateFormula();
               Assert.AreEqual(2, cells[0, 2].IntValue);
             }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(DateTime) {#putvalue_3}

Puts a DateTime value into the cell.

```csharp
public void PutValue(DateTime dateTime)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dateTime | DateTime | Input value |

### Remarks

Setting a DateTime value for a cell dose not means the cell will be formatted as date time automatically. DateTime value was maintained as numeric value in the data model of both ms excel and Aspose.Cells. Whether the numeric value will be taken as the numeric value itself or date time depends on the number format applied on this cell. If this cell has not been formatted as date time, it will be displayed as a numeric value even though what you input is DateTime.

### Examples

This example shows how to set DateTime value to a cell and make it be displayed as date time.

```csharp
[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

//Put date time into a cell
Cell cell = cells[0, 0];
cell.PutValue(new DateTime(2023, 5, 15));
Style style = cell.GetStyle(false);
style.Number = 14;
cell.SetStyle(style);
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(object) {#putvalue_4}

Puts an object value into the cell.

```csharp
public void PutValue(object objectValue)
```

| Parameter | Type | Description |
| --- | --- | --- |
| objectValue | Object | input value |

### Examples

```csharp
// Called: cells[2, 1].PutValue(new DateTime(now.Year, now.Month, now.Day));
private Workbook Method_Object_()
        {
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;
            cells[0, 0].Value = &quot;fruit&quot;;
            cells[1, 0].Value = &quot;grape&quot;;
            cells[2, 0].Value = &quot;blueberry&quot;;
            cells[3, 0].Value = &quot;kiwi&quot;;
            cells[4, 0].Value = &quot;cherry&quot;;
            cells[5, 0].Value = &quot;grape&quot;;
            cells[6, 0].Value = &quot;blueberry&quot;;
            cells[7, 0].Value = &quot;kiwi&quot;;
            cells[8, 0].Value = &quot;cherry&quot;;
            cells[9, 0].Value = &quot;grape&quot;;
            cells[10, 0].Value = &quot;blueberry&quot;;
            cells[11, 0].Value = &quot;kiwi&quot;;
            cells[12, 0].Value = &quot;cherry&quot;;

            DateTime now = DateTime.Now;

            Style s = book.CreateStyle();
            s.Number = 14;
            cells[0, 1].Value = &quot;year&quot;;
            cells[1, 1].PutValue(new DateTime(now.Year, now.Month, now.Day));
            cells[2, 1].PutValue(new DateTime(now.Year, now.Month, now.Day));
            cells[3, 1].PutValue(new DateTime(now.Year, now.Month, now.Day));
            cells[4, 1].PutValue(new DateTime(now.Year, now.Month, now.Day));
            cells[5, 1].PutValue(new DateTime(now.Year - 1, now.Month, now.Day));
            cells[6, 1].PutValue(new DateTime(now.Year - 1, now.Month, now.Day));
            cells[7, 1].PutValue(new DateTime(now.Year + 1, now.Month, now.Day));
            cells[8, 1].PutValue(new DateTime(now.Year + 1, now.Month, now.Day));
            cells[9, 1].PutValue(new DateTime(now.Year - 1, now.Month, now.Day));
            cells[10, 1].PutValue(new DateTime(now.Year - 1, now.Month, now.Day));
            cells[11, 1].PutValue(new DateTime(now.Year + 1, now.Month, now.Day));
            cells[12, 1].PutValue(new DateTime(now.Year + 1, now.Month, now.Day));            


            cells[1, 1].SetStyle(s);
            cells[2, 1].SetStyle(s);
            cells[3, 1].SetStyle(s);
            cells[4, 1].SetStyle(s);
            cells[5, 1].SetStyle(s);
            cells[6, 1].SetStyle(s);
            cells[7, 1].SetStyle(s);
            cells[8, 1].SetStyle(s);
            cells[9, 1].SetStyle(s);
            cells[10, 1].SetStyle(s);
            cells[11, 1].SetStyle(s);
            cells[12, 1].SetStyle(s);

            cells[0, 2].Value = &quot;amount&quot;;
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;
            cells[5, 2].Value = 90;
            cells[6, 2].Value = 100;
            cells[7, 2].Value = 110;
            cells[8, 2].Value = 120;
            cells[9, 2].Value = 110;
            cells[10, 2].Value = 120;
            cells[11, 2].Value = 110;
            cells[12, 2].Value = 120;
            return book;
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


