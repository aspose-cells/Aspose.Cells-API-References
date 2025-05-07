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
            tableLoadOption.Id = "id5";
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "id6";
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            Workbook wb = new Workbook(Constants.HtmlPath + "HtmlTableLoadOption.htm", loadOptions);
            wb.Save(_destFilesPath + "HtmlTableLoadOption1.xlsx");
            Assert.AreEqual("222aaa", wb.Worksheets[0].Cells["A1"].StringValue);
            Assert.AreEqual("333aaa", wb.Worksheets[0].Cells["A2"].StringValue);
            Assert.AreEqual("555aaa", wb.Worksheets[0].Cells["A4"].StringValue);
            Assert.AreEqual("666aaa", wb.Worksheets[0].Cells["A7"].StringValue);

            loadOptions.TableLoadOptions.Clear();
            loadOptions.TableLoadOptions.Add(0, 2);
            loadOptions.TableLoadOptions.Add(1, 0);
            loadOptions.TableLoadOptions.Add(2, 1);
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "id5";
            tableLoadOption.TargetSheetIndex= 0;
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "id6";
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            tableLoadOption.TargetSheetIndex = 1;
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "id4";
            tableLoadOption.TargetSheetIndex = 2;
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            wb = new Workbook(Constants.HtmlPath + "HtmlTableLoadOption.htm", loadOptions);
            wb.Save(_destFilesPath + "HtmlTableLoadOption2.xlsx");
            Assert.AreEqual("222bbb", wb.Worksheets[0].Cells["B1"].StringValue);
            Assert.AreEqual("555bbb", wb.Worksheets[0].Cells["B2"].StringValue);
            Assert.AreEqual("333bbb", wb.Worksheets[1].Cells["B1"].StringValue);
            Assert.AreEqual("666bbb", wb.Worksheets[1].Cells["B3"].StringValue);
            Assert.AreEqual("111ccc", wb.Worksheets[2].Cells["C1"].StringValue);
            Assert.AreEqual("444ccc", wb.Worksheets[2].Cells["C2"].StringValue);
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
// Called: loadOptions.TableLoadOptions.Add(2);
[Test]
        public void Method_Int32_()
        {
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.SupportDivTag = true;
            loadOptions.LoadFilter.LoadDataFilterOptions = LoadDataFilterOptions.Chart;
            loadOptions.TableLoadOptions.Add(1);
            loadOptions.TableLoadOptions.Add(2);
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "id5";
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "id6";
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            Workbook wb = new Workbook(Constants.HtmlPath + "HtmlTableLoadOption.htm", loadOptions);
            wb.Save(_destFilesPath + "HtmlTableLoadOption1.xlsx");
            Assert.AreEqual("222aaa", wb.Worksheets[0].Cells["A1"].StringValue);
            Assert.AreEqual("333aaa", wb.Worksheets[0].Cells["A2"].StringValue);
            Assert.AreEqual("555aaa", wb.Worksheets[0].Cells["A4"].StringValue);
            Assert.AreEqual("666aaa", wb.Worksheets[0].Cells["A7"].StringValue);

            loadOptions.TableLoadOptions.Clear();
            loadOptions.TableLoadOptions.Add(0, 2);
            loadOptions.TableLoadOptions.Add(1, 0);
            loadOptions.TableLoadOptions.Add(2, 1);
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "id5";
            tableLoadOption.TargetSheetIndex= 0;
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "id6";
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            tableLoadOption.TargetSheetIndex = 1;
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "id4";
            tableLoadOption.TargetSheetIndex = 2;
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            wb = new Workbook(Constants.HtmlPath + "HtmlTableLoadOption.htm", loadOptions);
            wb.Save(_destFilesPath + "HtmlTableLoadOption2.xlsx");
            Assert.AreEqual("222bbb", wb.Worksheets[0].Cells["B1"].StringValue);
            Assert.AreEqual("555bbb", wb.Worksheets[0].Cells["B2"].StringValue);
            Assert.AreEqual("333bbb", wb.Worksheets[1].Cells["B1"].StringValue);
            Assert.AreEqual("666bbb", wb.Worksheets[1].Cells["B3"].StringValue);
            Assert.AreEqual("111ccc", wb.Worksheets[2].Cells["C1"].StringValue);
            Assert.AreEqual("444ccc", wb.Worksheets[2].Cells["C2"].StringValue);
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
// Called: int index2 = tableLoadOptions.Add("tableId");
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
            int index2 = tableLoadOptions.Add("tableId");

            // Add a new HtmlTableLoadOption by table index and target sheet index
            int index3 = tableLoadOptions.Add(1, 1);

            // Add a new HtmlTableLoadOption by table id and target sheet index
            int index4 = tableLoadOptions.Add("tableId2", 2);

            // Add a new HtmlTableLoadOption by table index, target sheet index, and original sheet index
            int index5 = tableLoadOptions.Add(2, 2, 0);

            // Add a new HtmlTableLoadOption by table id, target sheet index, and original sheet index
            int index6 = tableLoadOptions.Add("tableId3", 3, 1);

            // Access the HtmlTableLoadOption at a specific index
            HtmlTableLoadOption option = tableLoadOptions[index1];

            // Set properties of the HtmlTableLoadOption
            option.TableIndex = 0;
            option.Id = "tableId";
            option.Name = "TableName";
            option.OriginalSheetIndex = 0;
            option.TargetSheetIndex = 1;
            option.TableToListObject = true;

            // Load an HTML file into the workbook using the load options
            workbook = new Workbook("HtmlTableLoadOptionCollectionExample_original.html", loadOptions);

            // Save the workbook
            workbook.Save("HtmlTableLoadOptionCollectionExample.xlsx");

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
// Called: loadOptions.TableLoadOptions.Add(1, 0);
[Test]
        public void Method_Int32_()
        {
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.SupportDivTag = true;
            loadOptions.LoadFilter.LoadDataFilterOptions = LoadDataFilterOptions.Chart;
            loadOptions.TableLoadOptions.Add(1);
            loadOptions.TableLoadOptions.Add(2);
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "id5";
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "id6";
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            Workbook wb = new Workbook(Constants.HtmlPath + "HtmlTableLoadOption.htm", loadOptions);
            wb.Save(_destFilesPath + "HtmlTableLoadOption1.xlsx");
            Assert.AreEqual("222aaa", wb.Worksheets[0].Cells["A1"].StringValue);
            Assert.AreEqual("333aaa", wb.Worksheets[0].Cells["A2"].StringValue);
            Assert.AreEqual("555aaa", wb.Worksheets[0].Cells["A4"].StringValue);
            Assert.AreEqual("666aaa", wb.Worksheets[0].Cells["A7"].StringValue);

            loadOptions.TableLoadOptions.Clear();
            loadOptions.TableLoadOptions.Add(0, 2);
            loadOptions.TableLoadOptions.Add(1, 0);
            loadOptions.TableLoadOptions.Add(2, 1);
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "id5";
            tableLoadOption.TargetSheetIndex= 0;
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "id6";
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            tableLoadOption.TargetSheetIndex = 1;
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "id4";
            tableLoadOption.TargetSheetIndex = 2;
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            wb = new Workbook(Constants.HtmlPath + "HtmlTableLoadOption.htm", loadOptions);
            wb.Save(_destFilesPath + "HtmlTableLoadOption2.xlsx");
            Assert.AreEqual("222bbb", wb.Worksheets[0].Cells["B1"].StringValue);
            Assert.AreEqual("555bbb", wb.Worksheets[0].Cells["B2"].StringValue);
            Assert.AreEqual("333bbb", wb.Worksheets[1].Cells["B1"].StringValue);
            Assert.AreEqual("666bbb", wb.Worksheets[1].Cells["B3"].StringValue);
            Assert.AreEqual("111ccc", wb.Worksheets[2].Cells["C1"].StringValue);
            Assert.AreEqual("444ccc", wb.Worksheets[2].Cells["C2"].StringValue);
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
// Called: int index4 = tableLoadOptions.Add("tableId2", 2);
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
            int index2 = tableLoadOptions.Add("tableId");

            // Add a new HtmlTableLoadOption by table index and target sheet index
            int index3 = tableLoadOptions.Add(1, 1);

            // Add a new HtmlTableLoadOption by table id and target sheet index
            int index4 = tableLoadOptions.Add("tableId2", 2);

            // Add a new HtmlTableLoadOption by table index, target sheet index, and original sheet index
            int index5 = tableLoadOptions.Add(2, 2, 0);

            // Add a new HtmlTableLoadOption by table id, target sheet index, and original sheet index
            int index6 = tableLoadOptions.Add("tableId3", 3, 1);

            // Access the HtmlTableLoadOption at a specific index
            HtmlTableLoadOption option = tableLoadOptions[index1];

            // Set properties of the HtmlTableLoadOption
            option.TableIndex = 0;
            option.Id = "tableId";
            option.Name = "TableName";
            option.OriginalSheetIndex = 0;
            option.TargetSheetIndex = 1;
            option.TableToListObject = true;

            // Load an HTML file into the workbook using the load options
            workbook = new Workbook("HtmlTableLoadOptionCollectionExample_original.html", loadOptions);

            // Save the workbook
            workbook.Save("HtmlTableLoadOptionCollectionExample.xlsx");

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
            int index2 = tableLoadOptions.Add("tableId");

            // Add a new HtmlTableLoadOption by table index and target sheet index
            int index3 = tableLoadOptions.Add(1, 1);

            // Add a new HtmlTableLoadOption by table id and target sheet index
            int index4 = tableLoadOptions.Add("tableId2", 2);

            // Add a new HtmlTableLoadOption by table index, target sheet index, and original sheet index
            int index5 = tableLoadOptions.Add(2, 2, 0);

            // Add a new HtmlTableLoadOption by table id, target sheet index, and original sheet index
            int index6 = tableLoadOptions.Add("tableId3", 3, 1);

            // Access the HtmlTableLoadOption at a specific index
            HtmlTableLoadOption option = tableLoadOptions[index1];

            // Set properties of the HtmlTableLoadOption
            option.TableIndex = 0;
            option.Id = "tableId";
            option.Name = "TableName";
            option.OriginalSheetIndex = 0;
            option.TargetSheetIndex = 1;
            option.TableToListObject = true;

            // Load an HTML file into the workbook using the load options
            workbook = new Workbook("HtmlTableLoadOptionCollectionExample_original.html", loadOptions);

            // Save the workbook
            workbook.Save("HtmlTableLoadOptionCollectionExample.xlsx");

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
// Called: int index6 = tableLoadOptions.Add("tableId3", 3, 1);
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
            int index2 = tableLoadOptions.Add("tableId");

            // Add a new HtmlTableLoadOption by table index and target sheet index
            int index3 = tableLoadOptions.Add(1, 1);

            // Add a new HtmlTableLoadOption by table id and target sheet index
            int index4 = tableLoadOptions.Add("tableId2", 2);

            // Add a new HtmlTableLoadOption by table index, target sheet index, and original sheet index
            int index5 = tableLoadOptions.Add(2, 2, 0);

            // Add a new HtmlTableLoadOption by table id, target sheet index, and original sheet index
            int index6 = tableLoadOptions.Add("tableId3", 3, 1);

            // Access the HtmlTableLoadOption at a specific index
            HtmlTableLoadOption option = tableLoadOptions[index1];

            // Set properties of the HtmlTableLoadOption
            option.TableIndex = 0;
            option.Id = "tableId";
            option.Name = "TableName";
            option.OriginalSheetIndex = 0;
            option.TargetSheetIndex = 1;
            option.TableToListObject = true;

            // Load an HTML file into the workbook using the load options
            workbook = new Workbook("HtmlTableLoadOptionCollectionExample_original.html", loadOptions);

            // Save the workbook
            workbook.Save("HtmlTableLoadOptionCollectionExample.xlsx");

            return;
        }
```

### See Also

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


