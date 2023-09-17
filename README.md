# win-traltq

Windows keyboard layout for Turkish, similar to macOS "Legacy Q" or Linux "Alt-Q"

This layout is useful for when you mostly input in US layout (for programming, English conversations, etc.)
but want to input Turkish characters occasionally, without having to switch the layout every time.

Other operating systems have this layout by default. macOS has the "Turkish Q Legacy" and Linux has "Turkish (Alt-Q)"
in most distributions. This repo attempts to bring the same experience to Windows.

There were similar repositories in GitHub, but none of them had the source (*.klc) file so I didn't want to install them.
Instead I made my own layout, which you can compile yourself.

## Building

1. Download [Microsoft Keyboard Layout Creator (MSKLC) Version 1.4](https://www.microsoft.com/en-US/download/details.aspx?id=102134)
2. Launch the Keyboard Layout Creator
3. Go to `File > Load Source File...` and load traltq.klc you downloaded from this repository.
4. (Optional) Review the layout and make edits as necessary.
5. Go to `Project > Build DLL and Setup Package`
6. Locate the installation folder (should be under Documents by default) and proceed with installation.

## Installation

1. Run setup.exe and complete the installation
2. Select the input method in Windows Settings (`Time & language > Typing`)

## Screenshots

![Layout01AltGr](https://github.com/bozbalci/win-traltq/assets/2644947/e943961c-837e-4be4-96e5-c0cbd2a532df)

![Layout01ShftAltGr](https://github.com/bozbalci/win-traltq/assets/2644947/5e62e63f-1558-4127-9ca3-61aa8711c823)

## Alternatives

If installing a Windows keyboard layout is not an option, you can also consider using my AutoHotkey script that achieves the same thing:

```ahk
!c::
SendInput ç
return

!+c::
SendInput Ç
return

!s::
SendInput ş
return

!+s::
SendInput Ş
return

!o::
SendInput ö
return

!+o::
SendInput Ö
return

!g::
SendInput ğ
return

!+g::
SendInput Ğ
return

!u::
SendInput ü
return

!+u::
SendInput Ü
return

!i::
SendInput ı
return

!+i::
SendInput İ
return

!t::
SendInput ₺
return

!+-::
SendInput —
return

!-::
SendInput –
return
```
