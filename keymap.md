# パッケージのキーバインド
更新とか再インストールとかしてるうちに、なんかよく分からんことになった。  
「date」「markdown-preview-plus」が使えないのは不便なので、新規設定と上書きしてみた。  


## date パッケージ
一番良く使う「YYYY-MM-DD」形式を `alt-ctrl-0` で。  
個人的に良く使うタイムスタンプ形式を `alt-ctrl-9` で。  
あまり使わないけど「HH:mm」形式 `alt-ctrl-8` で。  

まず、設定画面で表示させたい形式に変更する。  

[Date Format] YYYY-MM-DD  
[Time Format] HH:mm  
[Date Time Format] X

### date パッケージのキーバインド
下記の様に設定した。

```
'body':
  'alt-ctrl-0': 'date:date'
  'alt-ctrl-9': 'date:datetime'
  'alt-ctrl-8': 'date:time'
```


## markdown-preview パッケージ
Atom に基本で含まれているが「emmet」を入れてるので競合。  
ユーザーキーマップで上書きする。

```
'atom-text-editor, .markdown-preview':
  'ctrl-shift-M': 'markdown-preview:toggle'
```
