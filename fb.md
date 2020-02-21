## product sense:


1.There are two types of cars A and B. The number of people in US who use A and B are the same.  They drive the same distances each month.Now there are two new technologies, X and Y (of equal cost).If apply X, mpg of A would increase from 50 mpg to 75 mpg;If apply Y, mpg of B would increase from 10 mpg to 11 mpg.The goal is to decrease the dependence on foreign oil, or to decrease the consumption of gasoline. which technology would you apply?


2.fter applying the technology of your choice, assume there's money available for research on new technology, which car would you choose to conduct research on?


3.想在news feed里加一个reactions的功能，比如heart, smiley face。如果要present这个idea，应该如何scope，可以用那些现有数据back up

4.market champaign

5.表格里是国家，运营商，电话号，以及有多少人确认了电话号。问题就是围绕如果想提高电话号码的确认数应该怎样做

6.fb的推荐好友功能，当初设计这个功能要关注哪些metrics，以及可能存在的问题

7.如何设计FB的reaction，并且在没有做任何测试之前判定这个功能是否值得实施 （现在FB已经有了这个功能，假设回到若干年前，这个功能还在想法阶段

8.假设现在只有like一种reaction，设计一个metric来决定是否有需要增加除了like之外的reaction，怎么知道该加什么reaction

9.怎么提升『你可能认识的人』的功能

10.what data can you use to determine which reaction type it is.
How do you make sure the group have similar population. ez way?
what is the problem of random selecting?

11.How to get the nick name of each facebook user suach david - dave , and if we already have the data how can we use it?

12.打算给用户的发text notification 告诉他们close friends 的Update,评估这个Feature 值不值得加,注意是close, 然后问你有哪些Hypothesis（ 不是假设实验的hypothesis, 就是General的，比如User花更多时间在FB上之类的）
## SQL:

1.

| userid int | appid int | flag | ds |
|-------------|-------------|------------|--------------|

CTR click through rate
How to compute click-through rate (in mySQL)?
Now we know the rate is 1.4. What does it mean?

CTR的理解，如果CTR>1问LZ怎么办

2.第一个问题是给定一个data，包含每个post的类型，comment的原帖id，产生一个summary dataset，第一列是comment数，第二列是对应这个comment数的数目。没有限定语言，感觉很直接就拿SQL做了。后面还有followup问题是按post类型做那个summary dataset

3.cummulative clients table 和 今天所有clients table，更新今天的clients信息到cummulative table里。update flag （new clients，ressurrecting clients，churn，。。。）

4.怎么Update目前的table pool, 比如你想把今天的用户的table加到以往的所有的用户table里面

5.给两个table 一个是request（sender_id,request_id,time）
还有一个是accepts（accept_id, request_id,time）
求acceptance rate

6.给了一个table， 有postid， userid， post_type， comment_to， post_time
让算comments count的分布， 即comment数为0的有多少个post，为1的有多少个post。。。

7.friending (date | time | action | actor_id | target_id)
action = {'send_request','accept_request'}
Q(1):SQL to generate friend request acceptance rate
Q(2):generatethe friend request acceptance rate for people who accept within 24 hours:

8.content_actions:(ds,content_type{post,comment,photo},content_id,target_id) 求distribution of comment

9.
content_actions {user_id|content_id|conent_type|target_id} content_type = {"comment", "post"}
Q: 1.What is the total number of comments and total number of posts?
     2.what is the distribution of comments?



## Satisticas

1.如何跟business的人解释 p-value

2.排列组合概率问题

3.两个筛子一起扔，至少有一个是4的概率

## Other 
1.machine learning cluster



2.Determine whether a given string can be divided into a sequence of words, which should be in a dictionary. The function boolean isDictWord(String s) is given.
Implement the function boolean partition String(String s)


###
Q1. reverse print a linkedlist.

asked 3 methods. recursive, iterative, with-stack
. From 1point 3acres bbs
Q2. Design ReadLock and WriteLock.

Mulilple thread problem. When a reader is reading:
CALL
1.readlock()-baidu 1point3acres
2. to do something
3. readunlcok()  (when the reader completes reading)

when a writer is writing:
CALL
1. writelock()
2. to do something
3. writeunlock() (complete writing)

8.facebook privancy有个输入学校的地方，以前你可以随便输入任何东西， 甚至是乱码。你怎么确定输入的是真实的学校
   -how to find whether the high school in the Facebook privacyis the real one
   -how do you use thedata to manipulate it?

## Basic
why facebook？ why this position
然后让我讲一个做过的project