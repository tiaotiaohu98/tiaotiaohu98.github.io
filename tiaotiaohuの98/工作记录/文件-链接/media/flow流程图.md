```flow
st=>start: A
e=>end: B
op1=>operation: C
sub1=>subroutine: D
cond=>condition: E
io=>inputoutput: F
para=>parallel: G

st->op1->cond
cond(yes)->io->e
cond(no)->para
para(path1, bottom)->sub1(right)->op1
para(path2, top)->op1
```



```flow
st=>start: 开始
e=>end: 结束
op1=>operation: 步骤一
op2=>operation: 步骤二
op3=>operation: 步骤三
io=>inputoutput: 结束

st->op1->op2->op3->e
```



```flow
st=>start: 开始
e=>end: 结束
op1=>operation: 语句体
cond=>condition: 条件判断
st->cond
cond(true)->op1->e
cond(false)->e
```

