エヌ次元のコーディングスタイルを記述します。

# 命名について

## 英語を使う
命名は、基本的に英語で行います。

```
# NG
kiji
kizi

# OK
article
```

## 省略は使わない
命名に省略形を使わないでください。

```
# NG
artcl
art
init

# OK
article
initialize
```

## 関数・メソッド名は動詞を使う

```
# NG
initialization()

# OK
initialize()
```

## bool値の命名
慣習的に書かれているものを除き、基本的に bool 値 (true / false) は、ハンガリアン記法を使います。

```
# NG
editable
recommended

# OK
is_editable
is_recommended
should_be_logged_in
can_edit

# ただし、フレームワークなどの慣習で上記じゃない場合もある
primary
```

## 単数形と複数形は明確に
単数・複数は明確に区別します。 `List` (配列、リスト) や `Set` (集合) や、 `Map` (辞書、辞書型配列) は、複数形で記述してください。

また、一覧画面も、複数形を命名として使います。


```
# NG
user_list
userList
UserList
UserListPage

# OK
users_list  # または単に、 users
usersList
UsersList
UsersListPage
```

## 意味が伝わらない単語

意味 (セマンティック, semantic) の伝わらない単語は避ける。

```
# NG
data
information
content  # article.content (記事内容) などの場合は例外

# OK
body  # 本文という意味
detail  # 詳細という意味
response  # 応答という意味
payload  # 余計な情報を取り除いた後の、使いやすい形のデータ
article  # クラスがわかっているとき (この場合は Article) は、そのクラス名を素直に入れる
```

## キャメルケースとスネークケース、ハイフンつなぎ
基本的に、各言語の慣習や有名なコーディング規約に準じます。

CSS に関しては、次のようになります。

### CSSはハイフンつなぎ

```css
# NG
.user_profile
.UserDetail
.userIcon

# OK
.user-profile
.user-detail
.user-icon
```

過去のエヌ次元のプロダクトは、キャメルケースを使っていたこともあるので、その場合は例外とします。
