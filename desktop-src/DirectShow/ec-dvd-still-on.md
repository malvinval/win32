---
description: Signals the beginning of any still (PGC, Cell, or VOBU).
ms.assetid: cf2b08c9-22fa-4559-9289-787eaec46c6c
title: EC_DVD_STILL_ON (Dvdevcode.h)
ms.topic: reference
ms.date: 4/26/2023
topic_type: 
- APIRef
- kbSyntax
api_name: 
- EC_DVD_STILL_ON
api_type: 
- HeaderDef
api_location: 
- dvdevcode.h
ms.custom: UpdateFrequency5
---

# EC\_DVD\_STILL\_ON

\[The feature associated with this page, [DirectShow](/windows/win32/directshow/directshow), is a legacy feature. It has been superseded by [MediaPlayer](/uwp/api/Windows.Media.Playback.MediaPlayer) and [IMFMediaEngine](/windows/win32/api/mfmediaengine/nn-mfmediaengine-imfmediaengine). **MediaPlayer** and **IMFMediaEngine** have been optimized for Windows 10 and Windows 11. Microsoft strongly recommends that new code use **MediaPlayer** and **IMFMediaEngine** instead of **DirectShow**, when possible. Microsoft suggests that existing code that uses the legacy APIs be rewritten to use the new APIs if possible.\]

Signals the beginning of any still (PGC, Cell, or VOBU).

## Parameters

<dl> <dt>

<span id="lParam1"></span><span id="lparam1"></span><span id="LPARAM1"></span>*lParam1*
</dt> <dd>

Boolean (**BOOL**) value indicating whether buttons are available. Zero (0) indicates buttons are available so the [**IDvdControl2::StillOff**](/windows/desktop/api/Strmif/nf-strmif-idvdcontrol2-stilloff) method won't work. One (1) indicates no buttons are available, so **IDvdControl2::StillOff** will work.

</dd> <dt>

<span id="lParam2"></span><span id="lparam2"></span><span id="LPARAM2"></span>*lParam2*
</dt> <dd>

**DWORD** value indicating the number of seconds the still will last. 0xFFFFFFFF indicates an infinite still, meaning wait until the user presses a button or until the application calls [**IDvdControl2::StillOff**](/windows/desktop/api/Strmif/nf-strmif-idvdcontrol2-stilloff).

</dd> </dl>

## Remarks

All combinations of buttons and still are possible (buttons on with still on, buttons on with still off, button off with still on, button off with still off).

This event is raised in all domains.

## Requirements



| Requirement | Value |
|-------------------|----------------------------------------------------------------------------------------------------------|
| Header<br/> | <dl> <dt>Dvdevcode.h (include Dshow.h)</dt> </dl> |



## See also

<dl> <dt>

[DVD Applications](dvd-applications.md)
</dt> <dt>

[DVD Event Notification Codes](dvd-notification-codes.md)
</dt> <dt>

[Event Notification in DirectShow](event-notification-in-directshow.md)
</dt> </dl>

 

 




