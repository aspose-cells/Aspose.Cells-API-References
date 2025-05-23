---
title: Picture.IsDynamicDataExchange
second_title: Aspose.Cells for .NET API Reference
description: Picture property. Gets or sets whether dynamic data exchange
type: docs
url: /net/aspose.cells.drawing/picture/isdynamicdataexchange/
---
## Picture.IsDynamicDataExchange property

Gets or sets whether dynamic data exchange

```csharp
public bool IsDynamicDataExchange { get; set; }
```

### Examples

```csharp
// Called: image.IsDynamicDataExchange,
public void Picture_Property_IsDynamicDataExchange()
    {
           string path = Constants.sourcePath + "example.xls";
        Workbook workbook = new Workbook(path, new LoadOptions(LoadFormat.Excel97To2003));
     //   workbook.Worksheets[0].Pictures.Clear();
        List<CellsImageData> list = new List<CellsImageData>();

        for (int sheetNumber = 0; sheetNumber < workbook.Worksheets.Count; ++sheetNumber)
        {
            Worksheet sheet = workbook.Worksheets[sheetNumber];

            int numOfPictures = sheet.Pictures.Count;

            for (int imageCounter = 0; imageCounter < numOfPictures; ++imageCounter)
            {
                Picture image = sheet.Pictures[imageCounter];

                list.Add(new CellsImageData(
                                            sheetNumber,
                                            image.BorderWeight,
                                            image.Data,
                                            image.DisplayAsIcon,
                                            image.IsAutoSize,
                                            image.IsDynamicDataExchange,
                                            image.IsLink,
                                            image.SignatureLine,
                                            image.X,
                                            image.Y,
                                            image.UpperLeftRow,
                                            image.UpperLeftColumn,
                                            image.Height,
                                            image.Width,
                                            image.ZOrderPosition,
                                            image.Formula,
                                            image.Name));
            }

            sheet.Pictures.Clear();
        }


        workbook.Save(Constants.destPath + "example.xls");
        Workbook newworkbook = new Workbook(Constants.destPath + "example.xls", new LoadOptions(LoadFormat.Excel97To2003));

        foreach (CellsImageData imageData in list)
        {
            PictureCollection currentSheetPictureCollection = newworkbook.Worksheets[imageData.mSheetNumber].Pictures;
            int newPictureNumber = currentSheetPictureCollection.Add(imageData.mUpperLeftRow, imageData.mUpperLeftColumn, new MemoryStream(imageData.mData));
            Picture picture = newworkbook.Worksheets[imageData.mSheetNumber].Pictures[newPictureNumber];
            picture.X = imageData.mX;
            picture.Y = imageData.mY;
            picture.Height = imageData.mHeight;
            picture.Width = imageData.mWidth;
            picture.Formula = imageData.mFormula;
            picture.BorderWeight = imageData.mBorderWeight;
            picture.DisplayAsIcon = imageData.mDisplayAsIcon;
            picture.IsAutoSize = imageData.mIsAutoSize;
            picture.IsDynamicDataExchange = imageData.mIsDynamicDataExchange;
            picture.IsLink = imageData.mIsLink;
            picture.SignatureLine = imageData.mSignatureLine;
            picture.ZOrderPosition = imageData.mZOrderPosition;
            picture.Name = imageData.mName;
        }

        Util.SaveManCheck(newworkbook, "Shape", "example.xls");
     //   newworkbook.Save(path + "after.xlsafter.xls", Aspose.Cells.SaveFormat.Excel97To2003);
    }
```

### See Also

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


