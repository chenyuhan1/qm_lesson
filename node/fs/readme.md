# Promise

- node性能好 异步无阻塞的
    异步可以最快的放开对文件或者资源的控制
    IO， 数据库， 文件操作， 高访问时网站性能瓶颈， 文件要锁定
    readFileSync 其实就是在阻塞代码， 同一时刻拒绝了跟多的访问，

    文件的遍历查找， 异步的， 使用了readdirSync 同步阻塞式写法，
    1. src目录下找出所有的文件
        stat isFile| isDir
        2. 如果是文件， 就加入数组
            3. 目录需要再次重复去做第1步

    一 复杂事情， 分成n个s相似的加单事物，
    二 退出条件， 如果是文件，此为递归