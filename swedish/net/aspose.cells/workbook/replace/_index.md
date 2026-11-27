---
title: "Workbook.Replace"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Ersätter ett cellvärde med en ny sträng"
type: docs
url: /sv/net/aspose.cells/workbook/replace/
---
## Replace(string, string) {#replace_7}

Ersätter en cells värde med en ny string.

```csharp
public int Replace(string placeHolder, string newValue)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| platshållare | String | Cellplatshållare |
| nyttVärde | String | Strängvärde att ersätta |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Apple Orange");
            
            // Ersätt alla förekomster av "Apple" med "Mango"
            workbook.Replace("Apple", "Mango");
            
            // Spara arbetsboken
            workbook.Save("ReplaceDemo.xlsx");
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, int) {#replace_4}

Ersätter en cells värde med ett nytt integer.

```csharp
public int Replace(string placeHolder, int newValue)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| platshållare | String | Cellplatshållare |
| nyttVärde | Int32 | Heltalsvärde att ersätta |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Öppna första kalkylbladet och lägg till lite exempeldata
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("OriginalValue");
            worksheet.Cells["A2"].PutValue("OriginalValue");
            worksheet.Cells["A3"].PutValue("OriginalValue");
            
            // Ersätt alla förekomster av "OriginalValue" med heltalet 100
            workbook.Replace("OriginalValue", 100);
            
            // Spara arbetsboken
            workbook.Save("ReplacedWorkbook.xlsx");
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, double) {#replace_2}

Ersätter en cells värde med ett nytt double.

```csharp
public int Replace(string placeHolder, double newValue)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| platshållare | String | Cellplatshållare |
| nyttVärde | Double | Dubbelvärde att ersätta |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringDoubleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Placera lite exempeldata i celler
            worksheet.Cells["A1"].PutValue("AnOldValue");
            worksheet.Cells["A2"].PutValue("AnotherOldValue");
            worksheet.Cells["A3"].PutValue("AnOldValue");
            
            // Ersätt text med dubbelvärde
            double newValue = 100.0;
            workbook.Replace("AnOldValue", newValue);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, string[], bool) {#replace_9}

Ersätter en cells värde med en ny string‑array.

```csharp
public int Replace(string placeHolder, string[] newValues, bool isVertical)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| platshållare | String | Cellplatshållare |
| nyaVärden | String[] | Strängarray att ersätta |
| ärVertikal | Boolean | Sant - Vertikal, Falskt - Horisontell |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till lite exempeldata i celler
            worksheet.Cells["A1"].PutValue("AnOldValue");
            worksheet.Cells["A2"].PutValue("AnOldValue");
            worksheet.Cells["A3"].PutValue("AnOldValue");
            
            // Definiera nya värden att ersätta med
            string[] newValues = new string[] { "Tom", "Alice", "Jerry" };
            
            // Ersätt alla förekomster av "AnOldValue" med de nya värdena
            workbook.Replace("AnOldValue", newValues, true);
            
            // Spara arbetsboken
            workbook.Save("ReplaceDemo.xlsx");
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, int[], bool) {#replace_5}

Ersätter cellers värden med en integer‑array.

```csharp
public int Replace(string placeHolder, int[] newValues, bool isVertical)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| platshållare | String | Cellplatshållare |
| nyaVärden | Int32[] | Heltalsarray att ersätta |
| ärVertikal | Boolean | Sant - Vertikal, Falskt - Horisontell |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringInt32ArrayBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till lite exempeldata i celler
            worksheet.Cells["A1"].PutValue("OldValue");
            worksheet.Cells["A2"].PutValue("OldValue");
            worksheet.Cells["A3"].PutValue("OtherValue");
            
            // Definiera ersättningsvärden
            int[] newValues = new int[] { 1, 2, 3 };
            
            // Ersätt "OldValue" med arrayen av heltal
            workbook.Replace("OldValue", newValues, true);
            
            // Spara arbetsboken
            workbook.Save("ReplaceDemoOutput.xlsx");
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, double[], bool) {#replace_3}

Ersätter cellers värden med en double‑array.

```csharp
public int Replace(string placeHolder, double[] newValues, bool isVertical)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| platshållare | String | Cellplatshållare |
| nyaVärden | Double[] | Double-array att ersätta |
| ärVertikal | Boolean | Sant - Vertikal, Falskt - Horisontell |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringDoubleBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("AnOldValue");
            worksheet.Cells["A2"].PutValue("AnOldValue");
            worksheet.Cells["A3"].PutValue("AnOldValue");
            
            // Definiera ersättningsvärden
            double[] newValues = new double[] { 1.23, 2.56, 3.14159 };
            
            // Ersätt alla förekomster av "AnOldValue" med de nya värdena
            workbook.Replace("AnOldValue", newValues, true);
            
            // Spara arbetsboken
            workbook.Save("ReplaceDemoOutput.xlsx");
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, DataTable) {#replace_6}

Ersätter cellers värden med data från en DataTable.

```csharp
public int Replace(string placeHolder, DataTable insertTable)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| platshållare | String | Cellplatshållare |
| insertTable | DataTable | DataTable att ersätta |

### Exempel

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringDataTableDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Skapa en exempel-DataTable
            DataTable dataTable = new DataTable("Customers");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("City", typeof(string));
            
            // Lägg till exempeldata i DataTable
            dataTable.Rows.Add(1, "John Doe", "New York");
            dataTable.Rows.Add(2, "Jane Smith", "London");
            dataTable.Rows.Add(3, "Mike Johnson", "Paris");
            
            // Lägg till lite text i kalkylbladet som kommer att ersättas
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("CustomerData");
            
            // Ersätt texten med DataTable
            workbook.Replace("CustomerData", dataTable);
            
            // Spara arbetsboken
            workbook.Save("Output.xlsx");
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(bool, object) {#replace}

Ersätter cellers värden med ny data.

```csharp
public int Replace(bool boolValue, object newValue)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| boolValue | Boolean | Det booleska värdet som ska ersättas. |
| nyttVärde | Object | Nytt värde. Kan vara en sträng, ett heltal, en dubbel eller ett DateTime‑värde. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookMethodReplaceWithBooleanObjectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fyll i några celler med booleska värden
            worksheet.Cells["A1"].PutValue(true);
            worksheet.Cells["A2"].PutValue(false);
            worksheet.Cells["A3"].PutValue(true);
            
            try
            {
                // Anropa Replace‑metoden för att ersätta alla 'true'-värden med "REPLACED"
                int replacements = workbook.Replace(true, "REPLACED");
                
                Console.WriteLine($"Replaced {replacements} occurrences of 'true' with 'REPLACED'");
                
                // Visa resultaten
                Console.WriteLine("A1: " + worksheet.Cells["A1"].StringValue);
                Console.WriteLine("A2: " + worksheet.Cells["A2"].StringValue);
                Console.WriteLine("A3: " + worksheet.Cells["A3"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Replace method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("WorkbookMethodReplaceWithBooleanObjectDemo.xlsx");
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(int, object) {#replace_1}

Ersätter cellers värden med ny data.

```csharp
public int Replace(int intValue, object newValue)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| intValue | Int32 | Det heltalsvärde som ska ersättas. |
| nyttVärde | Object | Nytt värde. Kan vara en sträng, ett heltal, en dubbel eller ett DateTime‑värde. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookMethodReplaceWithInt32ObjectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fyll i några celler med heltalsvärden som ska ersättas
            worksheet.Cells["A1"].PutValue(100);
            worksheet.Cells["A2"].PutValue(200);
            worksheet.Cells["A3"].PutValue(100);
            
            try
            {
                // Anropa Replace‑metoden med parametrarna (Int32, Object)
                int replacements = workbook.Replace(100, "ReplacedValue");
                
                Console.WriteLine($"Replaced {replacements} occurrences of the value 100");
                
                // Visa kalkylbladets innehåll efter ersättning
                Console.WriteLine("Cell A1: " + worksheet.Cells["A1"].StringValue);
                Console.WriteLine("Cell A2: " + worksheet.Cells["A2"].StringValue);
                Console.WriteLine("Cell A3: " + worksheet.Cells["A3"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Replace method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("WorkbookMethodReplaceWithInt32ObjectDemo.xlsx");
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, string, ReplaceOptions) {#replace_8}

Ersätter en cells värde med en ny string.

```csharp
public int Replace(string placeHolder, string newValue, ReplaceOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| platshållare | String | Cellplatshållare |
| nyttVärde | String | Strängvärde att ersätta |
| alternativ | ReplaceOptions | Ersättningsalternativen |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringStringReplaceOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Hello World");
            sheet.Cells["A2"].PutValue("Hello Aspose");
            sheet.Cells["A3"].PutValue("Goodbye World");

            ReplaceOptions options = new ReplaceOptions
            {
                CaseSensitive = false,
                MatchEntireCellContents = false
            };

            int replacedCount = workbook.Replace("Hello", "Hi", options);

            Console.WriteLine($"Replacements made: {replacedCount}");
            workbook.Save("ReplaceDemo.xlsx");
        }
    }
}
```

### Se även

* class [ReplaceOptions](../../replaceoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


