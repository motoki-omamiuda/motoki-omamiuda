# linux-command
目次
> [grep](#grep)  
    ファイル内の文字列検索

> [find](#find)  
    特定の文字列を含むファイルを検索

<a id=grep></a>
## grep
ファイル内の文字列検索を行うコマンド  

このコマンドでは、`file_name.txt`から`search_string`を検索し、それがある行番号を出力している。  
```shell
grep -n 'search_string' file-name.txt
```

**-r**
ディレクトリとそのサブディレクトリ内の全ファイルを再帰的に検索
```shell
grep -r 'search_string' /path/
```

**-l**
検索文字列を含むファイルの名前のみを表示
```shell
grep -r -l 'search_string' /path/
```

<a id=find></a>
## find
特定の文字列を含むファイルを検索を行うコマンド
```shell
find /path/ -type f -name '*search_string*'
```
このコマンドでは、`search_string`をファイル名に含んだファイルを検索している。  
その他のオプション

**複数の条件で検索**
```shell
grep -r 'search_string' /path/
```
ディレクトリとそのサブディレクトリ内の全ファイルを再帰的に検索
