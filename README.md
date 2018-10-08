# coding-styles
エヌ次元のコーディングスタイルを記述します。

## 命名について

### 英語を使う
命名は、基本的に英語で行います。

```
# NG
kiji
kizi

# OK
article
```

### 省略は使わない
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

### 関数・メソッド名は動詞を使う

```
# NG
initialization()

# OK
initialize()
```

### 単数形と複数形は明確に
単数・複数は明確に区別します。 `List` (配列、リスト) や `Set` (集合) や、 `Map` (辞書、辞書型配列) は、複数形で記述してください。

また、一覧画面も、複数形を命名として使います。


```
# NG
user_list
userList
UserList
UserListPage

# OK
users_list
usersList
UsersList
UsersListPage
```
