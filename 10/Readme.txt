每种容器的使用场合
vector:比如软件历史记录的储存，我们经常需要查看历史记录，比如上一次记录，
        上上次记录，但却不会删除记录，因为纪录是事实的描述。

deque:比如排队购票，支持头部快速移除，尾部快速添加。vector头部删除时，会增加大量数据

vector和deque比较：
    1.vector.at（）比deque.at（）效率高
    2.如果有大量释放的操作，vector花的时间更少
    3.deque支持头部快速插入与快速移除，这是它的优点

queue:

list:比如公交乘客的储存，随时可能上下车，支持频繁的不确定位置元素的移除插入

set:比如对手机游戏的个人得分记录储存，储存要求高分到低分的顺序排列

map:比如按ID号储存10w个用户，想要快速ID查找对应的用户。如果使用vector，最坏可能要遍历整个空间