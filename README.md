# swap-ctrl-with-caps-lock

1. Press Win-r, open regedit
2. In Registry Editor, navigate to HKEY_LOCAL_MACHINE->SYSTEM->CurrentControlSet->Control->Keyboard Layout
3. Right click on 'Keyboard Layout', select New->Binary Value
4. Rename the file to 'Scancode Map'
5. Right click on the file 'Scancode Map', click Modify...
6. Enter the following values:

```
    00 00 00 00 00 00 00 00
    03 00 00 00 1D 00 3A 00
    3A 00 1D 00 00 00 00 00
```

7. Click OK
8. Restart computer
