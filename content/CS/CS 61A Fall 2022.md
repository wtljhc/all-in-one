---
Title: CS 61A Fall 2022
Description: 
Date: 2024-03-13
Draft: true
Weight: 1
aliases:
---
###### Updated on: Apr 15, 2024
<br>

https://inst.eecs.berkeley.edu/~cs61a/fa22/

包含内容：35个slide，31个相关文件，14个lab，14个discussion，10个homework，5个project。

>[!tip]+ 学习顺序：
>1. 看 Textbook
>2. 过一遍 PPT
>1. 看视频
>2. 做当天的 Lab/Disc/HW/Project
>3. 完成一周的阅读和练习，进行下一周
>4. 三次考试 Midterm（考试文件在右上角 Resources 处）
# Week 1
## 8.24

 >[!cite]+
 > 
 > [【Berkeley-CS61A-2022Fall】【精准空降到 22:07】]( https://www.bilibili.com/video/BV1GK411Q7qp/?share_source=copy_web&vd_source=862a9b866c7f942b0c19d0cf1f6fe15a&t=1327)
 > 
 > The course policy are that the point of this course is for people to learn, not to show off what they already know. For that reason, it's totally fine if you don't understand something yet. That the whole idea is that you have to practice, you have to work in it, in order to learn something well. 
 > 
 > And so I really don't tolerate students who give other students a hard time because they haven't mastered it yet, or who boast about how they compelted the homework in 10 minutes. That's not helpful. The point of this course is for people that spend on time on it to work on it and then to master the material through hard work.
 > 
 > ——[John DeNero](https://www.youtube.com/@JohnDeNero)

### Discussion 00: Getting Started

>[!cite]+
>
>[Discussion 0 | CS 61A Fall 2022 (berkeley.edu)](https://inst.eecs.berkeley.edu/~cs61a/fa22/disc/disc00/)
>
 > **Secrets to Success in CS 61A**
>
> 4. When stuck on a problem, try to ==verbally explain the area in which you are stuck.==
> 
>     This doesn't need to require a person who understands how to solve the problem (or even a person—this practice is often referred to as rubber ducking, since you can take a rubber duck and consider it your practice audience), because ==the main goal is for you to clarify your own thoughts and figure out where exactly you're getting stuck== with your understanding and code. From there you can focus on that portion to better your understanding.

### Lab 00: Getting Started

## 8.26

### Video

#### Names, Assignment, and User-Defined Functions

Three ways to bind name to values:
1. import
2. assignment operation（赋值）
3. def statement

#### Environment Diagrams

<font color="#ff0000">To visualize the interpreter's process.</font>
[Online Python Tutor - Composing Programs - Python 3](https://pythontutor.com/cp/composingprograms.html#mode=edit)
![image-20240129171221201.png](https://cdn.jsdelivr.net/gh/x-z-y/GitHubPic/202404091432124.png)

#### Defining Functions

```python
def <name>(<formal parameters>):
		return <return expression>
```

`Function signature` (First Line) and `Function body` (Everything indented after the first line)

![image.png](https://cdn.jsdelivr.net/gh/x-z-y/GitHubPic/202404091401398.png)

![image.png](https://cdn.jsdelivr.net/gh/x-z-y/GitHubPic/202404091402771.png)

>[!attention]
> So far, the current `Environment` (a sequence of `frames`, a `frame` is a binding between names and values) is either:
> 
>- `The global frame` alone, or
>- `A local frame`, **<u>followed</u>** by the global frame. (There's a sequence! )



If you want to look up names in Environment:

- look for that name in the local frame **first**
- If not found, look for it in the global fram.

