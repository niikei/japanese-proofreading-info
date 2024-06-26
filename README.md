# テキスト校正くん-niikei

[テキスト校正くん](https://marketplace.visualstudio.com/items?itemName=ICS.japanese-proofreading)の改良版です。

テキスト校正くんでは問題のある箇所がエラーとなるため、少し煩わしく感じることがありました。そこで、エラーを警告や情報の表示に変更できるようにしました。

[/src/rules/rule.ts](src/rules/rule.ts)の `severity` を適宜変更してください。  
`severity`の値とVS Code上に表示されるメッセージの対応は以下のとおりです。

- `severity = 0` : information
- `severity = 1` : warning
- `severity = 2` : error

### TODO
`severity` の値をユーザやワークスペースごとで設定可能にする。