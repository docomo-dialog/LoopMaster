# LoopMaster

LoopMasterは繰り返し処理や、<srai>と組み合わせて制限回数の設定などに使用することができます。  
また、LoopMasterが管理する情報はボット間で共有されるため、複数ボットを連携する際に役立ちます。  
<br/>
## 利用手順
1. ボットID「LoopMaster」でボットを作成  
   ボット編集にて"公開"をglobalもしくはpublicに設定
2. LoopMasterボットにLoopMaster.aimlを追加しデプロイ
3. 他のボットからsraixタグでLoopMasterボットを呼び出す  

<br/>

## 関数詳細
### ループインスタンス作成
###### 関数 : #NEW name limit
```
<sraix botid="(プロジェクト名)_LoopMaster">#NEW test 2</sraix>
```
ループインスタンスを作成します。  
"name" にはインスタンス名、"limit" にはループ回数を指定してください。  
上記の例の場合、ループ継続時は「continue」、ループ終了時は「break」の文字列が出力されます。  
<br/>
###### 関数 : #NEW name limit continue break
```
<sraix botid="(プロジェクト名)_LoopMaster">#NEW test 2 継続 終了</sraix>
```
ループの継続と終了の文字列を指定してループインスタンスを作成します。  
"continue" にはループ継続時に返す文字列、"break" には ループ終了時に返す文字列を指定してください。  
上記の例の場合、ループ継続時は「継続」、ループ終了時は「終了」の文字列が出力されます。  
<br/>
### ループ処理実行
###### 関数 : #LOOP name
```
<sraix botid="(プロジェクト名)_LoopMaster">#LOOP test</sraix>
```
ループ処理を行います。  
"name" にはインスタンス名を指定してください。  
<br/>
### ループインスタンス削除
###### 関数 : #DELETE name
```
<sraix botid="(プロジェクト名)_LoopMaster">#DELETE test</sraix>
```
ループインスタンスを削除します。
"name" にはインスタンス名を指定してください。

# Test Add
memo
