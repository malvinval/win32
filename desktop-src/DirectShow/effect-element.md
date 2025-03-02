---
description: The effect element defines an audio or video effect object. An effect is applied to a single stream (such as a composition, track, or source).
ms.assetid: aedb4491-f1f0-44b3-ad88-3fac8c90144d
title: effect Element (Gdipluseffects.h)
ms.topic: reference
ms.date: 4/26/2023
ms.custom: UpdateFrequency5
---

# effect Element

\[The feature associated with this page, [DirectShow](/windows/win32/directshow/directshow), is a legacy feature. It has been superseded by [MediaPlayer](/uwp/api/Windows.Media.Playback.MediaPlayer) and [IMFMediaEngine](/windows/win32/api/mfmediaengine/nn-mfmediaengine-imfmediaengine). **MediaPlayer** and **IMFMediaEngine** have been optimized for Windows 10 and Windows 11. Microsoft strongly recommends that new code use **MediaPlayer** and **IMFMediaEngine** instead of **DirectShow**, when possible. Microsoft suggests that existing code that uses the legacy APIs be rewritten to use the new APIs if possible.\]

> [!Note]  
> \[Deprecated. This API may be removed from future releases of Windows.\]

 

The `effect` element defines an audio or video effect object. An effect is applied to a single stream (such as a composition, track, or source).

## Attributes

[**clsid**](clsid-attribute.md), [**lock**](lock-attribute.md), [**mute**](mute-attribute.md), [**start**](start-attribute.md), [**stop**](stop-attribute.md), [**userdata**](userdata-attribute.md), [**userid**](userid-attribute.md), [**username**](username-attribute.md)

## Parent/Child Information



| Label | Value |
|----------|--------------------------------------------------------------------------------------------------------------------------------------|
| Parent   | [**composite**](composite-element.md), [**group**](group-element.md), [**clip**](clip-element.md), [**track**](track-element.md) |
| Children | [**param**](param-element.md)                                                                                                       |



 

## Remarks

The **clsid** attribute specifies the subobject that creates the effect.

## Examples


```XML
<effect clsid="{b05a941c-3ce1-11d2-952a-00c04fa34f05}" start="0" stop="32.0" />
```



## Requirements



| Requirement | Value |
|-------------------|---------------------------------------------------------------------------------------------|
| Header<br/> | <dl> <dt>Gdipluseffects.h</dt> </dl> |



## See also

<dl> <dt>

[XTL Elements](xtl-elements.md)
</dt> </dl>

 

 




