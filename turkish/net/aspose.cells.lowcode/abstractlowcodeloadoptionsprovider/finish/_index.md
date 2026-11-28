---
title: "AbstractLowCodeLoadOptionsProvider.Finish"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AbstractLowCodeLoadOptionsProvider yöntemi. Girdinin şu anki kısmını işledikten sonra kaynakları serbest bırakır"
type: docs
url: /tr/net/aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/finish/
---
## AbstractLowCodeLoadOptionsProvider.Finish method

Şu anda girişin işlenmiş kısmının ardından kaynakları serbest bırakır.

```csharp
public virtual void Finish(LowCodeLoadOptions part)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| parça | LowCodeLoadOptions | şu anda bölünmüş kısım için kullanılan yükleme seçenekleri. |

### Açıklamalar

Varsayılan olarak bu yöntem, yükleme seçenekleri bir Stream'i kaynak olarak belirttiğinde, [`InputStream`](../../lowcodeloadoptions/inputstream/) tarafından belirtilen akışı doğrudan kapatır. Kullanıcı, gereksinimlerine ve [`Current`](../current/) uygulamasına göre kaynakları nasıl serbest bırakacağını kontrol etmek için bu yöntemi geçersiz kılabilir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.Collections;

    public class AbstractLowCodeLoadOptionsProviderMethodFinishWithLowCodeLoadOptionsDemo
    {
        public static void Run()
        {
            string[] files = { "file1.xlsx", "file2.xlsx", "file3.xlsx" };

            CustomLoadOptionsProvider provider = new CustomLoadOptionsProvider(files);

            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
            saveOptions.OutputFile = "result.xlsx";
            saveOptions.SaveFormat = SaveFormat.Xlsx;

            LowCodeMergeOptions mergeOptions = new LowCodeMergeOptions();
            mergeOptions.LoadOptionsProvider = provider;
            mergeOptions.SaveOptions = saveOptions;

            SpreadsheetMerger.Process(mergeOptions);
        }
    }

    public class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
    {       

        public IEnumerator fileIter;
        public CustomLoadOptionsProvider(string[] files)
        {
            fileIter = files.GetEnumerator();
            current = new LowCodeLoadOptions();
        }
        private LowCodeLoadOptions current;

        public override LowCodeLoadOptions Current => current;

        public override bool MoveNext()
        {
            if (fileIter.MoveNext())
            {
                current = new LowCodeLoadOptions();
                current.InputFile = fileIter.Current.ToString();
                return true;
            }
            
            return false;
        }

        public override void Finish(LowCodeLoadOptions part)
        {
            base.Finish(part);
        }
    }
}
```

### Ayrıca Bakınız

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [AbstractLowCodeLoadOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


