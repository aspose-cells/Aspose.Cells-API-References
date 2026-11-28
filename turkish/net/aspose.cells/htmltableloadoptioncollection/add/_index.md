---
title: "HtmlTableLoadOptionCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlTableLoadOptionCollection yöntemi. Bu koleksiyona bir HtmlTableLoadOption ekler"
type: docs
url: /tr/net/aspose.cells/htmltableloadoptioncollection/add/
---
## Add(HtmlTableLoadOption) {#add}

Bu koleksiyona bir HtmlTableLoadOption ekler.

```csharp
[Obsolete("Use HtmlTableLoadOptionCollection.AddTableLoadOption(HtmlTableLoadOption) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(HtmlTableLoadOption item)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| öğe | HtmlTableLoadOption | bir HtmlTableLoadOption |

### Dönüş Değeri

eklenen öğenin indeksi

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen AddTableLoadOption() yöntemini kullanın. Bu yöntem, Aralık 2025'ten itibaren 6 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithHtmlTableLoadOptionDemo
    {
        public static void Run()
        {
            // HTML yükleme seçenekleri oluştur
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // Tablo yükleme seçenekleri ekle
            HtmlTableLoadOption tableLoadOption1 = new HtmlTableLoadOption();
            tableLoadOption1.Id = "table1";
            loadOptions.TableLoadOptions.Add(tableLoadOption1);

            HtmlTableLoadOption tableLoadOption2 = new HtmlTableLoadOption();
            tableLoadOption2.Id = "table2";
            tableLoadOption2.TargetSheetIndex = 1;
            loadOptions.TableLoadOptions.Add(tableLoadOption2);

            // Seçeneklerle çalışma kitabını yükle
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // Çıktıyı kaydet
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlTableLoadOption](../../htmltableloadoption/)
* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int) {#add_1}

Listeye bir HtmlTableLoadOption ekle.

```csharp
public int Add(int tableIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| tableIndex | Int32 | Tablo indeksi |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithInt32Demo
    {
        public static void Run()
        {
            // HtmlLoadOptions oluşturun
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // HtmlTableLoadOptionCollection örneğine erişin
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Tablo indeksine göre yeni bir HtmlTableLoadOption ekleyin
            int index = tableLoadOptions.Add(0);

            // Eklenen HtmlTableLoadOption öğesine erişin
            HtmlTableLoadOption option = tableLoadOptions[index];
            option.TableToListObject = true;

            // Seçeneklerle bir çalışma kitabı oluşturun ve HTML'yi yükleyin
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_4}

Listeye bir HtmlTableLoadOption ekle.

```csharp
public int Add(string tableId)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| tableId | String | Tablo ID'si |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            // HtmlLoadOptions oluşturun
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // HtmlTableLoadOptionCollection örneğine erişin
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Tablo kimliğine göre yeni bir HtmlTableLoadOption ekleyin
            int index = tableLoadOptions.Add("mainTable");

            // Eklenen HtmlTableLoadOption öğesine erişin
            HtmlTableLoadOption option = tableLoadOptions[index];
            option.TableToListObject = true;
            option.TargetSheetIndex = 0;

            // Çalışma kitabı oluşturun ve seçeneklerle HTML'yi yükleyin
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int) {#add_2}

Listeye bir HtmlTableLoadOption ekle.

```csharp
public int Add(int tableIndex, int targetSheetIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| tableIndex | Int32 | Tablo indeksi |
| targetSheetIndex | Int32 | Excel'deki çalışma sayfasının hedef indeksi |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // HTML yükleme seçenekleri oluştur
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // Hedef sayfa indeksiyle indekse göre tablolar ekle
            loadOptions.TableLoadOptions.Add(0, 2); // Table index 0 to sheet index 2
            loadOptions.TableLoadOptions.Add(1, 0); // Table index 1 to sheet index 0
            loadOptions.TableLoadOptions.Add(2, 1); // Table index 2 to sheet index 1

            // Belirtilen seçeneklerle HTML dosyasını yükleyin
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int) {#add_5}

Listeye bir HtmlTableLoadOption ekle.

```csharp
public int Add(string tableId, int targetSheetIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| tableId | String | Tablo ID'si |
| targetSheetIndex | Int32 | Excel'deki çalışma sayfasının hedef indeksi |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithStringInt32Demo
    {
        public static void Run()
        {
            // HtmlLoadOptions oluşturun
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // HtmlTableLoadOptionCollection örneğine erişin
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Tablo kimliği ve hedef sayfa indeksiyle yeni bir HtmlTableLoadOption ekleyin
            int index = tableLoadOptions.Add("tableId", 1);

            // Seçeneklerle bir çalışma kitabı oluşturun ve HTML'yi yükleyin
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, int) {#add_3}

Listeye bir HtmlTableLoadOption ekle.

```csharp
public int Add(int tableIndex, int targetSheetIndex, int originalSheetIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| tableIndex | Int32 | Tablo indeksi |
| targetSheetIndex | Int32 | Excel'deki çalışma sayfasının hedef indeksi |
| originalSheetIndex | Int32 | HTML'deki çalışma sayfasının orijinal indeksi |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // HtmlLoadOptions oluşturun
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // HtmlTableLoadOptionCollection öğesine erişin
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // İndeks 1, hedef sayfa indeksi 1 ve orijinal sayfa indeksi 0 olan bir tablo ekleyin
            int addedIndex = tableLoadOptions.Add(1, 1, 0);

            // Seçeneklerle bir çalışma kitabı oluşturun ve HTML'yi yükleyin
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Sonucu kaydet
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int) {#add_6}

Listeye bir HtmlTableLoadOption ekle.

```csharp
public int Add(string tableId, int targetSheetIndex, int originalSheetIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| tableId | String | Tablo ID'si |
| targetSheetIndex | Int32 | Excel'deki çalışma sayfasının hedef indeksi |
| originalSheetIndex | Int32 | HTML'deki çalışma sayfasının orijinal indeksi |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithStringInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // (String, Int32, Int32) parametreleriyle Add yöntemini gösterin
            int addedIndex = tableLoadOptions.Add("sampleTable", 1, 0);
            
            HtmlTableLoadOption option = tableLoadOptions[addedIndex];
            option.TableToListObject = true;

            // HTML dosyasını yükle (gerçek dosya yolu ile değiştirin)
            workbook = new Workbook("input.html", loadOptions);
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


