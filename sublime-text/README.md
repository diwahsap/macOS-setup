# Python di Sublime Text
## Langsung bisa jika tidak ada input-input-an
Sebenarnya Python bisa langsung digunakan, tekan **cmd + b**. Tetapi, jika kita membutuhkan input user, Sublime Text belum bisa. Kita harus mengatur terlebih dahulu.

## Cara mengatur supaya bisa input user
1. Buka Command Palette, ketik **cmd + shift + p**. Kemudian, ketik atau cari **Package Control: Install Package**.
2. Cari **Terminus**, dan Install Package.
3. Buka **Tools > Build System > New Build System**. Kemudian pastekan kode berikut:

```
{
  
  "target": "terminus_exec",
  "cancel": "terminus_cancel_build",

  "focus": true,

  "cmd": ["python3", "-u", "$file"],
  "file_regex": "^[ ]*File \"(...*?)\", line ([0-9]*)",
  "selector": "source.python"

}
```

4. Buka **Preferences > Package Settings > Terminus > Command Palette**. Ke.mudian pastekan kode berikut:

```
[
   {
        "caption": "Terminal (panel)",
        "command": "terminus_open",
        "args"   : {
           "cmd": "bash",
           "cwd": "${file_path:${folder}}",
           "title": "Command Prompt",
           "panel_name": "Terminus"
        }
   },
]  
```
5. Buka **Preferences > Package Settings > Terminus > Key Bindings**. Kemudian pastekan kode berikut:

```
[
   {
       "keys": ["alt+1"],
       "command": "terminus_open",
       "args" : {
           "cmd": "bash",
           "cwd": "${file_path:${folder}}",
           "panel_name": "Terminus"
       }
   }
] 
```
6. Buka **Tools > Build System > Python xxx**. Coba jalankan program Berhasil, seharusnya. Kita bisa langsung menggunakan Python input-input-an di Sublime Text.

## Referensi:
1. [How to Use Terminal in Sublime Text Editor ?](https://www.geeksforgeeks.org/how-to-use-terminal-in-sublime-text-editor/)
2. YouTube, tapi lupa.

