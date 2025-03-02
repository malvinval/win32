---
description: The put\_MaskName method specifies the name of a JPEG file to use as the wipe mask.
ms.assetid: f2b93c1e-479e-46c1-afe3-25b0ef720ab3
title: IDxtJpeg::put_MaskName method (Qedit.h)
ms.topic: reference
ms.date: 4/26/2023
topic_type: 
- APIRef
- kbSyntax
api_name: 
- IDxtJpeg.put_MaskName
api_type: 
- COM
api_location: 
- strmiids.lib
- strmiids.dll
ms.custom: UpdateFrequency5
---

# IDxtJpeg::put\_MaskName method

\[The feature associated with this page, [DirectShow](/windows/win32/directshow/directshow), is a legacy feature. It has been superseded by [MediaPlayer](/uwp/api/Windows.Media.Playback.MediaPlayer) and [IMFMediaEngine](/windows/win32/api/mfmediaengine/nn-mfmediaengine-imfmediaengine). **MediaPlayer** and **IMFMediaEngine** have been optimized for Windows 10 and Windows 11. Microsoft strongly recommends that new code use **MediaPlayer** and **IMFMediaEngine** instead of **DirectShow**, when possible. Microsoft suggests that existing code that uses the legacy APIs be rewritten to use the new APIs if possible.\]

> [!Note]  
> \[Deprecated. This API may be removed from future releases of Windows.\]

 

The `put_MaskName` method specifies the name of a JPEG file to use as the wipe mask. This mask will be used instead of one of the built-in wipe masks. The file must contain a monochrome, 8-bits-per-pixel gradient. The gradient is used as a mask to define the wipe's progression.

## Syntax


```C++
HRESULT put_MaskName(
  [in] BSTR newVal
);
```



## Parameters

<dl> <dt>

*newVal* \[in\]
</dt> <dd>

Specifies the name of the file.

</dd> </dl>

## Return value

If this method succeeds, it returns **S\_OK**. Otherwise, it returns an **HRESULT** error code.

## Remarks

To revert to a built-in mask, set the **MaskNum** property.

> [!Note]  
> The header file Qedit.h is not compatible with Direct3D headers later than version 7.

 

> [!Note]  
> To obtain Qedit.h, download the [Microsoft Windows SDK Update for Windows Vista and .NET Framework 3.0](https://msdn.microsoft.com/windowsvista/bb980924.aspx). Qedit.h is not available in the Microsoft Windows SDK for Windows 7 and .NET Framework 3.5 Service Pack 1.

 

## Requirements



| Requirement | Value |
|--------------------|-----------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>Qedit.h</dt> </dl>      |
| Library<br/> | <dl> <dt>Strmiids.lib</dt> </dl> |



## See also

<dl> <dt>

[**IDxtJpeg Interface**](idxtjpeg.md)
</dt> <dt>

[**IDxtJpeg::put\_MaskNum**](idxtjpeg-put-masknum.md)
</dt> </dl>

 

 




