# item_modifier-set_instrument
item_modifierの1項目であるset_instrumentのサンプルになります。

詳しくはブログ記事『[【マイクラ】コマンドで角笛の音色を変更する【item_modifiers】](https://natsumake.com/command_horn/)』を参考にしてください。

<h3>概要</h3>
角笛に対して、音色の指示ができます。<br>
具体的にはjsonファイル内で専用のタグを選択し、その中からランダムに1つの音が選ばれ、適用されます。

<h3>使い方</h3>

データパック導入後、ワールドに入り```/reload```と入力し実行してください。

タラを倒すことで、角笛をドロップし、その音色はset_instrumentによって決められています。

また、手元に角笛を持っている状態で以下のコマンドを実行することで、その音色を変更することが出来ます。

```copy
/item modify entity @s weapon.mainhand sample:set_instrument
```

以下のコマンドの場合は、参照するitem_modifierに音色を1種類しか指定していないタグを指定しているため、特定の音色に変化します。

```copy
/item modify entity @s weapon.mainhand sample:original_tag
```
