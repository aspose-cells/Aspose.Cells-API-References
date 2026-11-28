---
title: "WorksheetCollection.RegisterAddInFunction"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorksheetCollection yöntemi. Eklenti işlevini çalışma kitabına ekler"
type: docs
url: /tr/net/aspose.cells/worksheetcollection/registeraddinfunction/
---
## RegisterAddInFunction(string, string, bool) {#registeraddinfunction}

Eklenti işlevini çalışma kitabına ekler

```csharp
public int RegisterAddInFunction(string addInFile, string functionName, bool lib)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| addInFile | String | dosya eklenti işlevlerini içerir |
| functionName | String | eklentinin işlev adı |
| lib | Boolean | verilen addin dosyasının Workbook Add‑In kitaplığının dizininde veya alt dizininde olup olmadığı. Bu bayrak, verilen addInFile göreceli bir yol olduğunda etkili olur ve fark yaratır: true yolun Add‑In kitaplığına göreceli olduğunu, false ise yolun bu Workbook'a göreceli olduğunu gösterir. |

### Dönüş Değeri

Verilen eklenti işlevini içeren verinin ID'si

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRegisterAddInFunctionWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            
            // İlk çalışma sayfasını al
            Worksheet sheet = wb.Worksheets[0];
            
            // Örnek dosya yollarını ayarla (bunların ortamınızda mevcut olması gerekir)
            string addInFile1 = Path.Combine("AddIns", "MyAddIn1.xlam");
            string addInFile2 = Path.Combine("AddIns", "MyAddIn2.xlam");
            
            // Farklı parametrelerle eklenti işlevlerini kaydet
            int id1 = wb.Worksheets.RegisterAddInFunction(addInFile1, "MY_UDF1", false);
            int id2 = wb.Worksheets.RegisterAddInFunction(addInFile2, "MY_UDF2", true);
            
            // Kayıtlı işlevleri hücrelerde kullan
            sheet.Cells["A1"].Formula = "=MY_UDF1()";
            sheet.Cells["A2"].Formula = "=MY_UDF2()";
            
            // Çalışma kitabını kaydedin
            wb.Save("RegisterAddInFunctionDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RegisterAddInFunction(int, string) {#registeraddinfunction_1}

Eklenti işlevini çalışma kitabına ekler

```csharp
public string RegisterAddInFunction(int id, string functionName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| id | Int32 | Eklenti işlevlerini içeren verinin kimliği, aynı eklenti dosyası için `RegisterAddInFunction` ilk çağrısı ile elde edilebilir. |
| functionName | String | eklentinin işlev adı |

### Dönüş Değeri

Eklenti işlevlerini içeren eklenti dosyasının URL'si

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRegisterAddInFunctionWithInt32StringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk eklenti işlevini kaydedin ve kimliğini alın
            int functionId = workbook.Worksheets.RegisterAddInFunction("externallink1.xlam", "customfunc1", false);
            
            // Aynı kimliği kullanarak ikinci eklenti işlevini kaydedin
            workbook.Worksheets.RegisterAddInFunction(functionId, "customfunc2");
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Kayıtlı işlevleri formüllerde kullanın
            cells["A1"].Formula = "=customfunc1()";
            cells["A2"].Formula = "=customfunc2()";
            
            // Çalışma kitabını kaydedin
            workbook.Save("RegisterAddInFunctionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


