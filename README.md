# TestRepository
for the Test
```mermaid
flowchat
st=>start: 生产者线程进入 :>https://blog.csdn.net/qq_21808961
op1=>operation: 设置Info类的名称和内容
op2=>operation: 修改标志位
op3=>operation: 等待线程唤醒
op4=>operation: 等待消费者取走
cond=>condition: 判断标志位

st(right)->cond->op1->op2->op3
cond(yes,right)->op1
cond(no)->op4
```
