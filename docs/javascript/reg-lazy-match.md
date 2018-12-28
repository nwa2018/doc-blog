# 正则之最短匹配（懒惰匹配）

举个例子

字符串`aabab`匹配正则表达式`/a.*b/`的结果是整个字符串`aabab`，实际上我们只需要匹配到`aab`，这种默认的匹配形式叫做`贪婪匹配`，正则表达式通常会匹配`尽可能多`的字符

`懒惰匹配`只需要修改成`/a.*?b/`，即可匹配到字符`aab`，`懒惰匹配`意味着在匹配成功的前提下，尽可能少的重复

此外，正则表达式还有另一条规则，比懒惰／贪婪规则的优先级更高：最先开始的匹配拥有最高的优先权——The match that begins earliest wins

> 备注：[该分享](https://blog.csdn.net/liliflashfly/article/details/5331685)还有很多别的关于正则表达式的干货