---
title: HtmlTableLoadOptionCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: HtmlTableLoadOptionCollection method. Adds one HtmlTableLoadOption into this collection
type: docs
url: /net/aspose.cells/htmltableloadoptioncollection/add/
---
## Add(HtmlTableLoadOption) {#add}

Adds one HtmlTableLoadOption into this collection.

```csharp
public int Add(HtmlTableLoadOption item)
```

| Parameter | Type | Description |
| --- | --- | --- |
| item | HtmlTableLoadOption | one HtmlTableLoadOption |

### Return Value

the index of the added item

### Examples

```csharp
// Called: loadOptions.TableLoadOptions.Add(tableLoadOption);
[Test]
        public void Method_HtmlTableLoadOption_()
        {
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.SupportDivTag = true;
            loadOptions.LoadFilter.LoadDataFilterOptions = LoadDataFilterOptions.Chart;
            loadOptions.TableLoadOptions.Add(1);
            loadOptions.TableLoadOptions.Add(2);
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = &quot;id5&quot;;
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = &quot;id6&quot;;
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            Workbook wb = new Workbook(Constants.HtmlPath + &quot;HtmlTableLoadOption.htm&quot;, loadOptions);
            wb.Save(_destFilesPath + &quot;HtmlTableLoadOption1.xlsx&quot;);
            Assert.AreEqual(&quot;222aaa&quot;, wb.Worksheets[0].Cells[&quot;A1&quot;].StringValue);
            Assert.AreEqual(&quot;333aaa&quot;, wb.Worksheets[0].Cells[&quot;A2&quot;].StringValue);
            Assert.AreEqual(&quot;555aaa&quot;, wb.Worksheets[0].Cells[&quot;A4&quot;].StringValue);
            Assert.AreEqual(&quot;666aaa&quot;, wb.Worksheets[0].Cells[&quot;A7&quot;].StringValue);

            loadOptions.TableLoadOptions.Clear();
            loadOptions.TableLoadOptions.Add(0, 2);
            loadOptions.TableLoadOptions.Add(1, 0);
            loadOptions.TableLoadOptions.Add(2, 1);
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = &quot;id5&quot;;
            tableLoadOption.TargetSheetIndex= 0;
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = &quot;id6&quot;;
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            tableLoadOption.TargetSheetIndex = 1;
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = &quot;id4&quot;;
            tableLoadOption.TargetSheetIndex = 2;
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            wb = new Workbook(Constants.HtmlPath + &quot;HtmlTableLoadOption.htm&quot;, loadOptions);
            wb.Save(_destFilesPath + &quot;HtmlTableLoadOption2.xlsx&quot;);
            Assert.AreEqual(&quot;222bbb&quot;, wb.Worksheets[0].Cells[&quot;B1&quot;].StringValue);
            Assert.AreEqual(&quot;555bbb&quot;, wb.Worksheets[0].Cells[&quot;B2&quot;].StringValue);
            Assert.AreEqual(&quot;333bbb&quot;, wb.Worksheets[1].Cells[&quot;B1&quot;].StringValue);
            Assert.AreEqual(&quot;666bbb&quot;, wb.Worksheets[1].Cells[&quot;B3&quot;].StringValue);
            Assert.AreEqual(&quot;111ccc&quot;, wb.Worksheets[2].Cells[&quot;C1&quot;].StringValue);
            Assert.AreEqual(&quot;444ccc&quot;, wb.Worksheets[2].Cells[&quot;C2&quot;].StringValue);
        }
```

### See Also

* class [HtmlTableLoadOption](../../htmltableloadoption/)
* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int) {#add_1}

Add a HtmlTableLoadOption to the list.

```csharp
public int Add(int tableIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| tableIndex | Int32 | Table index |

### Examples

```csharp
// Called: loadOptions.TableLoadOptions.Add(1);
[Test]
        public void Method_Int32_()
        {
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.SupportDivTag = true;
            loadOptions.LoadFilter.LoadDataFilterOptions = LoadDataFilterOptions.Chart;
            loadOptions.TableLoadOptions.Add(1);
            loadOptions.TableLoadOptions.Add(2);
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = &quot;id5&quot;;
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = &quot;id6&quot;;
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            Workbook wb = new Workbook(Constants.HtmlPath + &quot;HtmlTableLoadOption.htm&quot;, loadOptions);
            wb.Save(_destFilesPath + &quot;HtmlTableLoadOption1.xlsx&quot;);
            Assert.AreEqual(&quot;222aaa&quot;, wb.Worksheets[0].Cells[&quot;A1&quot;].StringValue);
            Assert.AreEqual(&quot;333aaa&quot;, wb.Worksheets[0].Cells[&quot;A2&quot;].StringValue);
            Assert.AreEqual(&quot;555aaa&quot;, wb.Worksheets[0].Cells[&quot;A4&quot;].StringValue);
            Assert.AreEqual(&quot;666aaa&quot;, wb.Worksheets[0].Cells[&quot;A7&quot;].StringValue);

            loadOptions.TableLoadOptions.Clear();
            loadOptions.TableLoadOptions.Add(0, 2);
            loadOptions.TableLoadOptions.Add(1, 0);
            loadOptions.TableLoadOptions.Add(2, 1);
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = &quot;id5&quot;;
            tableLoadOption.TargetSheetIndex= 0;
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = &quot;id6&quot;;
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            tableLoadOption.TargetSheetIndex = 1;
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = &quot;id4&quot;;
            tableLoadOption.TargetSheetIndex = 2;
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            wb = new Workbook(Constants.HtmlPath + &quot;HtmlTableLoadOption.htm&quot;, loadOptions);
            wb.Save(_destFilesPath + &quot;HtmlTableLoadOption2.xlsx&quot;);
            Assert.AreEqual(&quot;222bbb&quot;, wb.Worksheets[0].Cells[&quot;B1&quot;].StringValue);
            Assert.AreEqual(&quot;555bbb&quot;, wb.Worksheets[0].Cells[&quot;B2&quot;].StringValue);
            Assert.AreEqual(&quot;333bbb&quot;, wb.Worksheets[1].Cells[&quot;B1&quot;].StringValue);
            Assert.AreEqual(&quot;666bbb&quot;, wb.Worksheets[1].Cells[&quot;B3&quot;].StringValue);
            Assert.AreEqual(&quot;111ccc&quot;, wb.Worksheets[2].Cells[&quot;C1&quot;].StringValue);
            Assert.AreEqual(&quot;444ccc&quot;, wb.Worksheets[2].Cells[&quot;C2&quot;].StringValue);
        }
```

### See Also

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_4}

Add a HtmlTableLoadOption to the list.

```csharp
public int Add(string tableId)
```

| Parameter | Type | Description |
| --- | --- | --- |
| tableId | String | Table ID |

### Examples

```csharp
// Called: int index2 = tableLoadOptions.Add(&amp;quot;tableId&amp;quot;);
public static void Method_String_()
        {
            // Create a new Workbook
            Workbook workbook = new Workbook();

            // Create HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Access the HtmlTableLoadOptionCollection instance
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Set the TableToListObject property
            tableLoadOptions.TableToListObject = true;

            // Add a new HtmlTableLoadOption by table index
            int index1 = tableLoadOptions.Add(0);

            // Add a new HtmlTableLoadOption by table id
            int index2 = tableLoadOptions.Add(&quot;tableId&quot;);

            // Add a new HtmlTableLoadOption by table index and target sheet index
            int index3 = tableLoadOptions.Add(1, 1);

            // Add a new HtmlTableLoadOption by table id and target sheet index
            int index4 = tableLoadOptions.Add(&quot;tableId2&quot;, 2);

            // Add a new HtmlTableLoadOption by table index, target sheet index, and original sheet index
            int index5 = tableLoadOptions.Add(2, 2, 0);

            // Add a new HtmlTableLoadOption by table id, target sheet index, and original sheet index
            int index6 = tableLoadOptions.Add(&quot;tableId3&quot;, 3, 1);

            // Access the HtmlTableLoadOption at a specific index
            HtmlTableLoadOption option = tableLoadOptions[index1];

            // Set properties of the HtmlTableLoadOption
            option.TableIndex = 0;
            option.Id = &quot;tableId&quot;;
            option.Name = &quot;TableName&quot;;
            option.OriginalSheetIndex = 0;
            option.TargetSheetIndex = 1;
            option.TableToListObject = true;

            // Load an HTML file into the workbook using the load options
            workbook = new Workbook(&quot;HtmlTableLoadOptionCollectionExample_original.html&quot;, loadOptions);

            // Save the workbook
            workbook.Save(&quot;HtmlTableLoadOptionCollectionExample.xlsx&quot;);

            return;
        }
```

### See Also

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int) {#add_2}

Add a HtmlTableLoadOption to the list.

```csharp
public int Add(int tableIndex, int targetSheetIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| tableIndex | Int32 | Table index |
| targetSheetIndex | Int32 | The target index of worksheet in Excel |

### Examples

```csharp
// Called: loadOptions.TableLoadOptions.Add(0, 2);
[Test]
        public void Method_Int32_()
        {
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.SupportDivTag = true;
            loadOptions.LoadFilter.LoadDataFilterOptions = LoadDataFilterOptions.Chart;
            loadOptions.TableLoadOptions.Add(1);
            loadOptions.TableLoadOptions.Add(2);
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = &quot;id5&quot;;
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = &quot;id6&quot;;
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            Workbook wb = new Workbook(Constants.HtmlPath + &quot;HtmlTableLoadOption.htm&quot;, loadOptions);
            wb.Save(_destFilesPath + &quot;HtmlTableLoadOption1.xlsx&quot;);
            Assert.AreEqual(&quot;222aaa&quot;, wb.Worksheets[0].Cells[&quot;A1&quot;].StringValue);
            Assert.AreEqual(&quot;333aaa&quot;, wb.Worksheets[0].Cells[&quot;A2&quot;].StringValue);
            Assert.AreEqual(&quot;555aaa&quot;, wb.Worksheets[0].Cells[&quot;A4&quot;].StringValue);
            Assert.AreEqual(&quot;666aaa&quot;, wb.Worksheets[0].Cells[&quot;A7&quot;].StringValue);

            loadOptions.TableLoadOptions.Clear();
            loadOptions.TableLoadOptions.Add(0, 2);
            loadOptions.TableLoadOptions.Add(1, 0);
            loadOptions.TableLoadOptions.Add(2, 1);
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = &quot;id5&quot;;
            tableLoadOption.TargetSheetIndex= 0;
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = &quot;id6&quot;;
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            tableLoadOption.TargetSheetIndex = 1;
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = &quot;id4&quot;;
            tableLoadOption.TargetSheetIndex = 2;
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            wb = new Workbook(Constants.HtmlPath + &quot;HtmlTableLoadOption.htm&quot;, loadOptions);
            wb.Save(_destFilesPath + &quot;HtmlTableLoadOption2.xlsx&quot;);
            Assert.AreEqual(&quot;222bbb&quot;, wb.Worksheets[0].Cells[&quot;B1&quot;].StringValue);
            Assert.AreEqual(&quot;555bbb&quot;, wb.Worksheets[0].Cells[&quot;B2&quot;].StringValue);
            Assert.AreEqual(&quot;333bbb&quot;, wb.Worksheets[1].Cells[&quot;B1&quot;].StringValue);
            Assert.AreEqual(&quot;666bbb&quot;, wb.Worksheets[1].Cells[&quot;B3&quot;].StringValue);
            Assert.AreEqual(&quot;111ccc&quot;, wb.Worksheets[2].Cells[&quot;C1&quot;].StringValue);
            Assert.AreEqual(&quot;444ccc&quot;, wb.Worksheets[2].Cells[&quot;C2&quot;].StringValue);
        }
```

### See Also

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int) {#add_5}

Add a HtmlTableLoadOption to the list.

```csharp
public int Add(string tableId, int targetSheetIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| tableId | String | Table ID |
| targetSheetIndex | Int32 | The target index of worksheet in Excel |

### Examples

```csharp
// Called: int index4 = tableLoadOptions.Add(&amp;quot;tableId2&amp;quot;, 2);
public static void Method_Int32_()
        {
            // Create a new Workbook
            Workbook workbook = new Workbook();

            // Create HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Access the HtmlTableLoadOptionCollection instance
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Set the TableToListObject property
            tableLoadOptions.TableToListObject = true;

            // Add a new HtmlTableLoadOption by table index
            int index1 = tableLoadOptions.Add(0);

            // Add a new HtmlTableLoadOption by table id
            int index2 = tableLoadOptions.Add(&quot;tableId&quot;);

            // Add a new HtmlTableLoadOption by table index and target sheet index
            int index3 = tableLoadOptions.Add(1, 1);

            // Add a new HtmlTableLoadOption by table id and target sheet index
            int index4 = tableLoadOptions.Add(&quot;tableId2&quot;, 2);

            // Add a new HtmlTableLoadOption by table index, target sheet index, and original sheet index
            int index5 = tableLoadOptions.Add(2, 2, 0);

            // Add a new HtmlTableLoadOption by table id, target sheet index, and original sheet index
            int index6 = tableLoadOptions.Add(&quot;tableId3&quot;, 3, 1);

            // Access the HtmlTableLoadOption at a specific index
            HtmlTableLoadOption option = tableLoadOptions[index1];

            // Set properties of the HtmlTableLoadOption
            option.TableIndex = 0;
            option.Id = &quot;tableId&quot;;
            option.Name = &quot;TableName&quot;;
            option.OriginalSheetIndex = 0;
            option.TargetSheetIndex = 1;
            option.TableToListObject = true;

            // Load an HTML file into the workbook using the load options
            workbook = new Workbook(&quot;HtmlTableLoadOptionCollectionExample_original.html&quot;, loadOptions);

            // Save the workbook
            workbook.Save(&quot;HtmlTableLoadOptionCollectionExample.xlsx&quot;);

            return;
        }
```

### See Also

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, int) {#add_3}

Add a HtmlTableLoadOption to the list.

```csharp
public int Add(int tableIndex, int targetSheetIndex, int originalSheetIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| tableIndex | Int32 | Table index |
| targetSheetIndex | Int32 | The target index of worksheet in Excel |
| originalSheetIndex | Int32 | The original index of worksheet in the html |

### Examples

```csharp
// Called: int index5 = tableLoadOptions.Add(2, 2, 0);
public static void Method_Int32_()
        {
            // Create a new Workbook
            Workbook workbook = new Workbook();

            // Create HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Access the HtmlTableLoadOptionCollection instance
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Set the TableToListObject property
            tableLoadOptions.TableToListObject = true;

            // Add a new HtmlTableLoadOption by table index
            int index1 = tableLoadOptions.Add(0);

            // Add a new HtmlTableLoadOption by table id
            int index2 = tableLoadOptions.Add(&quot;tableId&quot;);

            // Add a new HtmlTableLoadOption by table index and target sheet index
            int index3 = tableLoadOptions.Add(1, 1);

            // Add a new HtmlTableLoadOption by table id and target sheet index
            int index4 = tableLoadOptions.Add(&quot;tableId2&quot;, 2);

            // Add a new HtmlTableLoadOption by table index, target sheet index, and original sheet index
            int index5 = tableLoadOptions.Add(2, 2, 0);

            // Add a new HtmlTableLoadOption by table id, target sheet index, and original sheet index
            int index6 = tableLoadOptions.Add(&quot;tableId3&quot;, 3, 1);

            // Access the HtmlTableLoadOption at a specific index
            HtmlTableLoadOption option = tableLoadOptions[index1];

            // Set properties of the HtmlTableLoadOption
            option.TableIndex = 0;
            option.Id = &quot;tableId&quot;;
            option.Name = &quot;TableName&quot;;
            option.OriginalSheetIndex = 0;
            option.TargetSheetIndex = 1;
            option.TableToListObject = true;

            // Load an HTML file into the workbook using the load options
            workbook = new Workbook(&quot;HtmlTableLoadOptionCollectionExample_original.html&quot;, loadOptions);

            // Save the workbook
            workbook.Save(&quot;HtmlTableLoadOptionCollectionExample.xlsx&quot;);

            return;
        }
```

### See Also

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int) {#add_6}

Add a HtmlTableLoadOption to the list.

```csharp
public int Add(string tableId, int targetSheetIndex, int originalSheetIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| tableId | String | Table ID |
| targetSheetIndex | Int32 | The target index of worksheet in Excel |
| originalSheetIndex | Int32 | The original index of worksheet in the html |

### Examples

```csharp
// Called: int index6 = tableLoadOptions.Add(&amp;quot;tableId3&amp;quot;, 3, 1);
public static void Method_Int32_()
        {
            // Create a new Workbook
            Workbook workbook = new Workbook();

            // Create HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Access the HtmlTableLoadOptionCollection instance
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Set the TableToListObject property
            tableLoadOptions.TableToListObject = true;

            // Add a new HtmlTableLoadOption by table index
            int index1 = tableLoadOptions.Add(0);

            // Add a new HtmlTableLoadOption by table id
            int index2 = tableLoadOptions.Add(&quot;tableId&quot;);

            // Add a new HtmlTableLoadOption by table index and target sheet index
            int index3 = tableLoadOptions.Add(1, 1);

            // Add a new HtmlTableLoadOption by table id and target sheet index
            int index4 = tableLoadOptions.Add(&quot;tableId2&quot;, 2);

            // Add a new HtmlTableLoadOption by table index, target sheet index, and original sheet index
            int index5 = tableLoadOptions.Add(2, 2, 0);

            // Add a new HtmlTableLoadOption by table id, target sheet index, and original sheet index
            int index6 = tableLoadOptions.Add(&quot;tableId3&quot;, 3, 1);

            // Access the HtmlTableLoadOption at a specific index
            HtmlTableLoadOption option = tableLoadOptions[index1];

            // Set properties of the HtmlTableLoadOption
            option.TableIndex = 0;
            option.Id = &quot;tableId&quot;;
            option.Name = &quot;TableName&quot;;
            option.OriginalSheetIndex = 0;
            option.TargetSheetIndex = 1;
            option.TableToListObject = true;

            // Load an HTML file into the workbook using the load options
            workbook = new Workbook(&quot;HtmlTableLoadOptionCollectionExample_original.html&quot;, loadOptions);

            // Save the workbook
            workbook.Save(&quot;HtmlTableLoadOptionCollectionExample.xlsx&quot;);

            return;
        }
```

### See Also

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


