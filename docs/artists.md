## 歌手单曲
说明: 获取前50首热门歌曲和部分歌手信息

必选参数:

```id```: 歌手id

**接口地址:**```/api/artists/song```

**调用例子:**```/api/artists/song?id=6452```

## 歌手专辑

必选参数:

```id```: 歌手id

可选参数:

```limit```: 返回数量, 默认为50

```offset```: 偏移数量，用于分页, 如:```(页数 - 1) * 50```, 其中```50```为```limit```的值, 默认为0

**接口地址:**```/api/artists/album```

**调用例子:**```/api/artists/album?id=6452&limit=10```


### 最新专辑
说明: 没有特定的歌手，所有专辑中最新的那几张

无参数

**接口地址:**```/api/artists/album/new```

### 获取专辑内容

必选参数:

```id```: 专辑id

**接口地址:**```/api/artists/album/detail```

**调用例子:**```/api/artists/album/detail?id=2301158```


### 专辑动态信息
说明: 获取专辑的喜欢数，转发数，收藏数等

必选参数:

```id```: 专辑id

**接口地址:**```/api/artists/album/dynamic```

**调用例子:**```/api/artists/album/dynamic?id=2301158```

### 收藏/取消收藏专辑
说明: 需登录

必选参数:

```id```: 专辑id

可选参数:

```t```: 1 收藏 （默认） 0 取消收藏

**接口地址:**```/api/artists/album/sub```

**调用例子:**```/api/artists/album/sub?id=2301158&t=0```指取消收藏id为2301158的专辑

### 获取已收藏专辑列表
说明: 需登录

可选参数:

```limit```: 返回数量, 默认为30

```offset```: 偏移数量，用于分页, 如:```(页数 - 1) * 30```, 其中```30```为```limit```的值, 默认为0

**接口地址:**```/api/artists/album/sublist```

## 歌手详情

必选参数:

```id```: 歌手id

**接口地址:**```/api/artists/desc```

**调用例子:**```/api/artists/desc?id=6452```

## 歌手MV

必选参数:

```id```: 歌手id

可选参数:

```limit```: 返回数量, 默认为30

```offset```: 偏移数量，用于分页, 如:```(页数 - 1) * 30```, 其中```30```为```limit```的值, 默认为0

**接口地址:**```/api/artists/mv```

**调用例子:**```/api/artists/mv?id=6452&limit=10```


## 热门歌手

可选参数:

```limit```: 返回数量, 默认为30

```offset```: 偏移数量，用于分页, 如:```(页数 - 1) * 30```, 其中```30```为```limit```的值, 默认为0

**接口地址:**```/api/artists/top```


## 获取相似歌手

必选参数:

```id```: 歌手id

**接口地址:**```/api/artists/simi```

**调用例子:**```/api/artists/simi?id=6452```

## 歌手分类列表

可选参数:

```cat```: 歌手分类参数，默认为1001（华语男歌手）

```init```: 按首字母索引查找参数，默认为空

```limit```: 返回数量, 默认为30

```offset```: 偏移数量，用于分页, 如:```(页数 - 1) * 30```, 其中```30```为```limit```的值, 默认为0

所有歌手分类参数:

    华语男歌手 1001

    华语女歌手 1002

    华语组合/乐队 1003

    欧美男歌手 2001

    欧美女歌手 2002

    欧美组合/乐队 2003

    其他男歌手 4001

    其他女歌手 4002

    其他组合/乐队 4003

    入驻歌手 5001

    日本男歌手 6001

    日本女歌手 6002

    日本组合/乐队 6003

    韩国男歌手 7001

    韩国女歌手 7002

    韩国组合/乐队 7003

**接口地址:**```/api/artists/lists```

**调用例子:**```/api/artists/lists?cat=1002&init=c```指查找拼音首字母为C的华语女歌手

## 收藏/取消收藏歌手
说明: 需登录

必选参数:

```id```: 歌手id

可选参数:

```t```: 收藏或取消收藏 (默认为1 收藏) 0 为取消收藏

**接口地址:**```/api/artists/sub```

**调用例子:**```/api/artists/sub?id=6452&t=0```指取消收藏id为6452的歌手

## 收藏的歌手列表
说明: 需登录

可选参数:

```limit```: 返回数量, 默认为30

```offset```: 偏移数量，用于分页, 如:```(页数 - 1) * 30```, 其中```30```为```limit```的值, 默认为0

**接口地址:**```/api/artists/sublist```

## 歌手热门50首歌曲

必选参数:

```id```: 歌手id

**接口地址:**```/api/artists/topsong```

**调用例子:**```/api/artists/topsong?id=6452```

## 歌手榜
说明: 获取人气最高的歌手

无参数

**接口地址:**```/api/artists/toplist```