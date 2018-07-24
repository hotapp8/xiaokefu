# xiaokefu
芝麻小客服接入示例
## 打开客服
```
<button type='default' open-type='contact'> 打开客服 (普通客服) </button>
```
## 固定的客服头像和昵称
``` 
<button type='default' session-from='{"nickName":"赵丽颖","avatarUrl":"https://ss0.baidu.com/6ONWsjip0QIZ8tyhnq/it/u=956547549,964120469&fm=58"}' open-type="contact"> 带头像客服 （固定头像）</button>
``` 

## 通过后端传递用户的头像和昵称
```
<button type='default' session-from='{"nickName":"{{userInfo.nickName}}","avatarUrl":"{{userInfo.avatarUrl}}"}' open-type="contact" >带头像客服（微信头像）</button>
```
## 传递用户浏览哪个产品，跟踪用户来源
```
<button type='default' session-from='{"source":"产品BBBB","nickName":"{{userInfo.nickName}}","avatarUrl":"{{userInfo.avatarUrl}}"}' open-type="contact" >指定消息来源</button>
```
## 指定客服
```
<button type='default' session-from='{"kefu":["126","127"],"nickName":"{{userInfo.nickName}}","avatarUrl":"{{userInfo.avatarUrl}}"}' open-type="contact"> 指定客服</button>
```
## 卡片消息
```
<button open-type='contact' send-message-title="会话内消息卡片" send-message-path="/pages/index/index" send-message-img="https://imgsa.baidu.com/baike/pic/item/562c11dfa9ec8a13918d4ed4fb03918fa0ecc06b.jpg" show-message-card="true">卡片消息</button>
```
