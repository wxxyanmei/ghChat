# react-chat

![image](https://user-images.githubusercontent.com/24861316/42560354-0d569eb0-8529-11e8-924f-948bdc786426.png)

![image](https://user-images.githubusercontent.com/24861316/42560447-414e6676-8529-11e8-99c5-97ecf12b3d77.png)

![image](https://user-images.githubusercontent.com/24861316/42560766-09b51858-852a-11e8-9eb0-0a6d78857a5a.png)


目前进度

- [x] 登录
- [x] 注册
- [x] 弹窗，提示等组件
- [x] 响应式布局。以前的实现只是移动端的布局。
- [x] 机器人智能聊天回复
- [x] 聊天页表
- [x] 私聊（外加重要的重构）：始化时请求聊天列表所有聊天对象的聊天记录（后期将请求聊天记录的限制为20条聊天内容，避免初始化时间过长），接着根据点击列表导致chatId(取自url params)的改变，重新渲染新的聊天内容。以前的实现方式是点击进入每个聊天页面都会发1至多次请求然后渲染页面，性能较差。。。终于想出自己较为满意的方案，开森~ 不过现在看以前vue-chat的代码真是烂成💩了，搞完react-chat有空了回去重构一波
- [x] 群聊 && 重构： 本来是根据消息列表上的群和好友去遍历发HTTP请求拿数据，现在直接在后端整合好一次性用websocket发过来，减少请求次数且websocket在此情况性能更优一些； 完成群聊功能
- [ ] 把后端接口封装成sdk
