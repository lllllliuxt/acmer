# 机试笔记

记录学习acm的技巧和内容
***
### 机试经验
- [经验1](https://github.com/lllllliuxt/acmer/blob/master/%E6%9C%BA%E8%AF%95%E8%B5%84%E6%96%99%E6%89%93%E5%8D%B0.docx)
- #include <bits/stdc++.h> 万能包
- abs()求绝对值
- #### ip问题的经验
  - 输出的大小写要注意一致
  - scanf的格式化输入启发很大，节省很多
  - while（T--）
  - sscanf()的使用
- 字符串转换为指定进制的数
```c++
 int stoInt(string s,int jz){                    //将一个字符串转换为指定进制的数
    int res=0;
    for(int i=0;i<s.length();i++){
        int tmp;
        if(s[i]-'0'>=0 && s[i]-'0'<=9){
            tmp=s[i]-'0';
        }else{
            tmp=s[i]-'A'+10;
        }
        res=res*jz+tmp;
    }
    return res;
}
```
***
### 北邮机试题

- [ip问题](https://github.com/lllllliuxt/acmer/blob/master/%E5%8C%97%E9%82%AE%E6%9C%BA%E8%AF%95/ip%E9%97%AE%E9%A2%98)

- [合法ip](https://github.com/lllllliuxt/acmer/blob/master/%E5%8C%97%E9%82%AE%E6%9C%BA%E8%AF%95/%E5%90%88%E6%B3%95ip.md)

- [统计节点个数](https://github.com/lllllliuxt/acmer/blob/master/%E5%8C%97%E9%82%AE%E6%9C%BA%E8%AF%95/%E7%BB%9F%E8%AE%A1%E8%8A%82%E7%82%B9%E4%B8%AA%E6%95%B0.md)
- [中序遍历序列](https://github.com/lllllliuxt/acmer/blob/master/%E5%8C%97%E9%82%AE%E6%9C%BA%E8%AF%95/%E4%B8%AD)
- [中位数](https://github.com/lllllliuxt/acmer/blob/master/%E5%8C%97%E9%82%AE%E6%9C%BA%E8%AF%95/%E4%B8%AD%E4%BD%8D%E6%95%B0.md)
- [内存分配](https://github.com/lllllliuxt/acmer/blob/master/%E5%8C%97%E9%82%AE%E6%9C%BA%E8%AF%95/%E5%86%85%E5%AD%98%E5%88%86%E9%85%8D.md)
- [图像识别](https://github.com/lllllliuxt/acmer/blob/master/北邮机试/图像识别.md)
- [字符串转换](https://github.com/lllllliuxt/acmer/blob/master/北邮机试/字符串转换.md)
- [最小距离查询](https://github.com/lllllliuxt/acmer/blob/master/北邮机试/最小距离查询.md)
- [统计节点个数](https://github.com/lllllliuxt/acmer/blob/master/北邮机试/统计节点个数.md)
- [汇编](https://github.com/lllllliuxt/acmer/blob/master/北邮机试/汇编.md)
- [最长等差子序列](https://github.com/lllllliuxt/acmer/blob/master/%E5%8C%97%E9%82%AE%E6%9C%BA%E8%AF%95/%E6%9C%80%E9%95%BF%E8%BF%9E%E7%BB%AD%E7%AD%89%E5%B7%AE%E5%AD%90%E5%BA%8F%E5%88%97.md)
- [最近公共祖先](https://github.com/lllllliuxt/acmer/blob/master/%E5%8C%97%E9%82%AE%E6%9C%BA%E8%AF%95/%E6%9C%80%E8%BF%91%E5%85%AC%E5%85%B1%E7%A5%96%E5%85%88.md)
- [进程管理](https://github.com/lllllliuxt/acmer/blob/master/%E5%8C%97%E9%82%AE%E6%9C%BA%E8%AF%95/%E8%BF%9B%E7%A8%8B%E7%AE%A1%E7%90%86.md)
- [图像压缩存储](https://github.com/lllllliuxt/acmer/blob/master/%E5%8C%97%E9%82%AE%E6%9C%BA%E8%AF%95/%E5%9B%BE%E5%83%8F%E5%8E%8B%E7%BC%A9%E5%AD%98%E5%82%A8.md)
