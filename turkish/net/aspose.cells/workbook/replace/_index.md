---
title: "Workbook.Replace"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Bir hücrenin değerini yeni bir dizeyle değiştirir"
type: docs
url: /tr/net/aspose.cells/workbook/replace/
---
## Replace(string, string) {#replace_7}

Bir hücrenin değerini yeni bir string ile değiştirir.

```csharp
public int Replace(string placeHolder, string newValue)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| Yer tutucu | String | Hücre yer tutucu |
| yeniDeğer | String | Değiştirilecek dize değeri |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelere örnek veri ekle
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Apple Orange");
            
            // Tüm "Apple" oluşumlarını "Mango" ile değiştir
            workbook.Replace("Apple", "Mango");
            
            // Çalışma kitabını kaydedin
            workbook.Save("ReplaceDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, int) {#replace_4}

Bir hücrenin değerini yeni bir integer ile değiştirir.

```csharp
public int Replace(string placeHolder, int newValue)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| Yer tutucu | String | Hücre yer tutucu |
| yeniDeğer | Int32 | Değiştirilecek tam sayı değeri |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş ve bazı örnek veriler ekle
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("OriginalValue");
            worksheet.Cells["A2"].PutValue("OriginalValue");
            worksheet.Cells["A3"].PutValue("OriginalValue");
            
            // Tüm "OriginalValue" oluşumlarını tam sayı 100 ile değiştir
            workbook.Replace("OriginalValue", 100);
            
            // Çalışma kitabını kaydedin
            workbook.Save("ReplacedWorkbook.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, double) {#replace_2}

Bir hücrenin değerini yeni bir double ile değiştirir.

```csharp
public int Replace(string placeHolder, double newValue)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| Yer tutucu | String | Hücre yer tutucu |
| yeniDeğer | Double | Değiştirilecek Double değer |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringDoubleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelere bazı örnek veriler ekle
            worksheet.Cells["A1"].PutValue("AnOldValue");
            worksheet.Cells["A2"].PutValue("AnotherOldValue");
            worksheet.Cells["A3"].PutValue("AnOldValue");
            
            // Metni double değerle değiştir
            double newValue = 100.0;
            workbook.Replace("AnOldValue", newValue);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, string[], bool) {#replace_9}

Bir hücrenin değerini yeni bir string dizisiyle değiştirir.

```csharp
public int Replace(string placeHolder, string[] newValues, bool isVertical)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| Yer tutucu | String | Hücre yer tutucu |
| newValues | String[] | Değiştirilecek String dizisi |
| isVertical | Boolean | True - Dikey, False - Yatay |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelere bazı örnek veriler ekle
            worksheet.Cells["A1"].PutValue("AnOldValue");
            worksheet.Cells["A2"].PutValue("AnOldValue");
            worksheet.Cells["A3"].PutValue("AnOldValue");
            
            // Değiştirmek için yeni değerleri tanımla
            string[] newValues = new string[] { "Tom", "Alice", "Jerry" };
            
            // Tüm "AnOldValue" oluşumlarını yeni değerlerle değiştir
            workbook.Replace("AnOldValue", newValues, true);
            
            // Çalışma kitabını kaydedin
            workbook.Save("ReplaceDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, int[], bool) {#replace_5}

Hücrelerin değerlerini bir integer dizisiyle değiştirir.

```csharp
public int Replace(string placeHolder, int[] newValues, bool isVertical)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| Yer tutucu | String | Hücre yer tutucu |
| newValues | Int32[] | Değiştirilecek Integer dizisi |
| isVertical | Boolean | True - Dikey, False - Yatay |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringInt32ArrayBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelere bazı örnek veriler ekle
            worksheet.Cells["A1"].PutValue("OldValue");
            worksheet.Cells["A2"].PutValue("OldValue");
            worksheet.Cells["A3"].PutValue("OtherValue");
            
            // Değiştirme değerlerini tanımla
            int[] newValues = new int[] { 1, 2, 3 };
            
            // "OldValue" öğesini tam sayı dizisiyle değiştir
            workbook.Replace("OldValue", newValues, true);
            
            // Çalışma kitabını kaydedin
            workbook.Save("ReplaceDemoOutput.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, double[], bool) {#replace_3}

Hücrelerin değerlerini bir double dizisiyle değiştirir.

```csharp
public int Replace(string placeHolder, double[] newValues, bool isVertical)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| Yer tutucu | String | Hücre yer tutucu |
| newValues | Double[] | Değiştirilecek Double dizisi |
| isVertical | Boolean | True - Dikey, False - Yatay |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringDoubleBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelere örnek veri ekle
            worksheet.Cells["A1"].PutValue("AnOldValue");
            worksheet.Cells["A2"].PutValue("AnOldValue");
            worksheet.Cells["A3"].PutValue("AnOldValue");
            
            // Değiştirme değerlerini tanımla
            double[] newValues = new double[] { 1.23, 2.56, 3.14159 };
            
            // Tüm "AnOldValue" oluşumlarını yeni değerlerle değiştir
            workbook.Replace("AnOldValue", newValues, true);
            
            // Çalışma kitabını kaydedin
            workbook.Save("ReplaceDemoOutput.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, DataTable) {#replace_6}

Hücrelerin değerlerini bir DataTable'dan gelen verilerle değiştirir.

```csharp
public int Replace(string placeHolder, DataTable insertTable)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| Yer tutucu | String | Hücre yer tutucu |
| insertTable | DataTable | Değiştirilecek DataTable |

### Örnekler

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
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Örnek bir DataTable oluştur
            DataTable dataTable = new DataTable("Customers");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("City", typeof(string));
            
            // DataTable'a örnek veri ekle
            dataTable.Rows.Add(1, "John Doe", "New York");
            dataTable.Rows.Add(2, "Jane Smith", "London");
            dataTable.Rows.Add(3, "Mike Johnson", "Paris");
            
            // Değiştirilecek worksheet'a bazı metinler ekle
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("CustomerData");
            
            // Metni DataTable ile değiştir
            workbook.Replace("CustomerData", dataTable);
            
            // Çalışma kitabını kaydedin
            workbook.Save("Output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(bool, object) {#replace}

Hücrelerin değerlerini yeni verilerle değiştirir.

```csharp
public int Replace(bool boolValue, object newValue)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| boolValue | Boolean | Değiştirilecek boolean değer. |
| yeniDeğer | Object | Yeni değer. String, integer, double veya DateTime değeri olabilir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookMethodReplaceWithBooleanObjectDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bazı hücreleri boolean değerlerle doldurun
            worksheet.Cells["A1"].PutValue(true);
            worksheet.Cells["A2"].PutValue(false);
            worksheet.Cells["A3"].PutValue(true);
            
            try
            {
                // Replace metodunu çağırarak tüm 'true' değerlerini "REPLACED" ile değiştirin
                int replacements = workbook.Replace(true, "REPLACED");
                
                Console.WriteLine($"Replaced {replacements} occurrences of 'true' with 'REPLACED'");
                
                // Sonuçları görüntüleyin
                Console.WriteLine("A1: " + worksheet.Cells["A1"].StringValue);
                Console.WriteLine("A2: " + worksheet.Cells["A2"].StringValue);
                Console.WriteLine("A3: " + worksheet.Cells["A3"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Replace method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("WorkbookMethodReplaceWithBooleanObjectDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(int, object) {#replace_1}

Hücrelerin değerlerini yeni verilerle değiştirir.

```csharp
public int Replace(int intValue, object newValue)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| intValue | Int32 | Değiştirilecek integer değeri. |
| yeniDeğer | Object | Yeni değer. String, integer, double veya DateTime değeri olabilir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookMethodReplaceWithInt32ObjectDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Değiştirilecek integer değerlerle bazı hücreleri doldurun
            worksheet.Cells["A1"].PutValue(100);
            worksheet.Cells["A2"].PutValue(200);
            worksheet.Cells["A3"].PutValue(100);
            
            try
            {
                // Replace metodunu (Int32, Object) parametreleriyle çağırın
                int replacements = workbook.Replace(100, "ReplacedValue");
                
                Console.WriteLine($"Replaced {replacements} occurrences of the value 100");
                
                // Değiştirmeden sonra çalışma sayfası içeriğini gösterin
                Console.WriteLine("Cell A1: " + worksheet.Cells["A1"].StringValue);
                Console.WriteLine("Cell A2: " + worksheet.Cells["A2"].StringValue);
                Console.WriteLine("Cell A3: " + worksheet.Cells["A3"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Replace method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("WorkbookMethodReplaceWithInt32ObjectDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, string, ReplaceOptions) {#replace_8}

Bir hücrenin değerini yeni bir string ile değiştirir.

```csharp
public int Replace(string placeHolder, string newValue, ReplaceOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| Yer tutucu | String | Hücre yer tutucu |
| yeniDeğer | String | Değiştirilecek dize değeri |
| seçenekler | ReplaceOptions | Değiştirme seçenekleri |

### Örnekler

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

### Ayrıca Bakınız

* class [ReplaceOptions](../../replaceoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


