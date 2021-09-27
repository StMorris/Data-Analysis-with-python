## Programming Language Analysis
<img src='https://github.com/StMorris/Data-Analysis-with-python/blob/main/Programming%20language%20Analysis/prog.jpg' 
     style = "width:800px;height:500px"/>


## Get the Data

Either use the provided .csv file or (optionally) get fresh (the freshest?) data from running an SQL query on StackExchange: 

The data used for this analysis contains number of times a programming language is mentioned in posts over time on stack overflow, from 1st of July 2008  to 1st of September 2021.

Follow this link to run the query from StackExchange (https://data.stackexchange.com/stackoverflow/query/675441/popular-programming-languages-per-over-time-eversql-com) to get your own .csv file

<code>
select dateadd(month, datediff(month, 0, q.CreationDate), 0) m, TagName, count(*)
from PostTags pt
join Posts q on q.Id=pt.PostId
join Tags t on t.Id=pt.TagId
where TagName in ('java','c','c++','python','c#','javascript','assembly','php','perl','ruby','visual basic','swift','r','object-c','scratch','go','swift','delphi')
and q.CreationDate < dateadd(month, datediff(month, 0, getdate()), 0)
group by dateadd(month, datediff(month, 0, q.CreationDate), 0), TagName
order by dateadd(month, datediff(month, 0, q.CreationDate), 0)
</code>



-  The oldest programming language still in use today is FORTRAN, which was developed in 1957. Since then many other programming languages have been developed. But which programming language is the most popular? Which programming language is the Kim Kardashian of programming languages; the one people just can't stop talking about? 

- StackOverflow will help us answer this burning question. Each post on Stack OverFlow comes with a Tag. And this Tag can be the name of a programming language.

- To figure out which language is the most popular, all we need to do is count the number of posts on Stack Overflow that are tagged with each language. The language with the most posts wins!
  
## Analysis
  
  - The most popular language from 2020 to 2021 by the number of posts is python, followed by javascript.
  - The most popular programming language from 2008 to 2012 by the number of posts is c# followed by Java.
  - The most popular programming language from 2015 to 2018 by the number of posts is javascript.
