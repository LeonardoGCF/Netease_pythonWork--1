'''
统计如下字符串 str 中每个单词出现的次数，结果存入 dict 中，单词为 key，次数为 value，
并按照 value 由高到底排序，输出此 dict。
'''
import re
str = """ The Zen of Python, by Tim Peters Beautiful is better than ugly.
Explicit is better than implicit.
Simple is better than complex.
Complex is better than complicated. Flat is better than nested.
Sparse is better than dense.
Readability counts.
Special cases aren't special enough to break the rules.
Although practicality beats purity.
Errors should never pass silently.
Unless explicitly silenced.
In the face of ambiguity, refuse the temptation to guess.
There should be one-- and preferably only one --obvious way to do it. Although that way may not be obvious at first unless you're Dutch. Now is better than never.
Although never is often better than *right* now.
If the implementation is hard to explain, it's a bad idea.
If the implementation is easy to explain, it may be a good idea. Namespaces are one honking great idea -- let's do more of those! """

#Step1: clear the string 只保留单词
string = re.sub(r'[^\w\s]','',str)
#Step2: count every word and join to the dict
Result = {word : string.split().count(word) for word in set(string.split())}
#step3: sort and print
result = sorted(Result.items(), key = lambda kv:(kv[1], kv[0]),reverse=True)
print (result)


