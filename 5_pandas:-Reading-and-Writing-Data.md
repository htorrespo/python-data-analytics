<!--
https://link-springer-com.ezproxy.unal.edu.co/chapter/10.1007/978-1-4842-3913-1_5
-->

# pandas: Reading and Writing Data

In the previous chapter, you became familiar with the pandas library and with the basic functiona lities that it provides for data analysis. You saw that dataframe and series are the heart of this library. These are the material on which to perform all data manipulations, calculations, and analysis.

In this chapter, you will see all of the tools provided by pandas for reading data stored in many types of media (such as files and databases). In parallel, you will also see how to write data structures directly on these formats, without worrying too much about the technologies used.

This chapter focuses on a series of I/O API functions that pandas provides to read and write data directly as datafram e objects. We start by looking at text files, then move gradually to more complex binary formats.

At the end of the chapter, you’ll also learn how to interface with all common databases, both SQL and NoSQL, including examples that show how to store data in a dataframe. At the same time, you learn how to read data contained in a database and retrieve them as a dataframe.

## I/O API Tools

pandas is a library specialized for data analysis, so you expect that it is mainly focused on calculation and data processing. The processes of writing and reading data from/to external files can be considered part of data processing. In fact, you will see how, even at this stage, you can perform some operations in order to prepare the incoming data for manipulation.

Thus, this step is very important for data analysis and therefore a specific tool for this purpose must be present in the library pandas—a set of functions called I/O API. These functions are divided into two main categories: readers and writers.

```
Readers          Writers

read_csv         to_csv
read_excel       to_excel
read_hdf         to_hdf
read_sql         to_sql
read_json        to_json
read_html        to_html
read_stata       to_stata
read_clipboard   to_clipboard
read_pickle      to_pickle
read_msgpack     to_msgpack (experimental)
read_gbq         to_gbq (experimental)
```
