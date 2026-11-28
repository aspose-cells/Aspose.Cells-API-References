---
title: "AbstractLowCodeSaveOptionsProvider.Finish"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AbstractLowCodeSaveOptionsProvider yöntemi. Şu anda bölünmüş parçayı işledikten sonra kaynakları serbest bırakır"
type: docs
url: /tr/net/aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/
---
## AbstractLowCodeSaveOptionsProvider.Finish method

Şu anda bölünmüş parçayı işledikten sonra kaynakları serbest bırakır.

```csharp
public virtual void Finish(LowCodeSaveOptions part)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| parça | LowCodeSaveOptions | şu anda bölünmüş parça için kullanılan kaydetme seçenekleri. |

### Açıklamalar

Varsayılan olarak bu yöntem, kaydetme seçenekleri bir Stream'i hedef olarak belirlemişse, [`OutputStream`](../../lowcodesaveoptions/outputstream/) tarafından belirtilen akışı doğrudan kapatır. Kullanıcı, gereksinimlerine ve [`GetSaveOptions`](../getsaveoptions/) uygulamasına göre kaynakları nasıl serbest bırakacağını kontrol etmek için bu yöntemi geçersiz kılabilir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeSaveOptionsProviderMethodFinishWithLowCodeSaveOptionsDemo
    {
        public static void Run()
        {

            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            loadOptions.InputFile = "split.xlsx";

            // Somut sağlayıcı örneği oluşturun
            var provider = new CustomLowCodeSaveOptionsProvider();

            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
            splitOptions.SaveOptionsProvider = provider;
            splitOptions.LoadOptions = loadOptions;

            SpreadsheetSplitter.Process(splitOptions);
                     
          
        }
    }

    // AbstractLowCodeSaveOptionsProvider'ın somut uygulaması
    public class CustomLowCodeSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override void Finish(LowCodeSaveOptions part)
        { 
            base.Finish(part);
        }
        // Gerekli soyut yöntemi uygulayın
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            LowCodeSaveOptions result = new LowCodeSaveOptions();
            result.SaveFormat = SaveFormat.Xlsx;
            result.OutputFile = partInfo.SheetName + "_split.xlsx";
            Console.WriteLine(result.OutputFile);
            return result;
        }
    }
}
```

### Ayrıca Bakınız

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [AbstractLowCodeSaveOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


