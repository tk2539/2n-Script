# 2n Script

## ファイル

- main.py => コアこれを実行する

- commandlist.md => 2n Scriptで使えるコマンドリスト

- run_2n.bat => Windowsの2nパッチ

- run_2n.command => Macの2nパッチ

- omikuji.2n => 2n Scriptで書かれたテストのおみくじアプリ

## コマンドリスト

- 基本
    - `input x = 1`
    - `output x`
    - `print "Hello world!"`

- 条件分岐
    - `?(x > 0)`
    - `if ?(x > 5) {}`
    - `else if ?(x == 3) {}`
    - `else {}`

- リストとランダム
    - `addlist list.x = 1,2,3`
    - `output list.x`
    - `input x = random[1,2,3]`
    - `input y = random[list.x]`

- ループ
    - `for 10 {}`
    - `while {break}`

- 関数
    - `function sayHello {print "Hello"}`
    - `action sayHello()`

- JSON連携
    - `import.json test.json`
    - ```
    operation test {

    addlist list.x = json.getkey scores

    getlist list.x = json.addkey results

    }

    ```

- サブスクリプト
    - `import.2n submodule.2n`

- ネスト処理
    - while

    {

        if ?(x == 1)

        {

            break

        }

    }


- コメントアウト
    - "#"を先頭に入力