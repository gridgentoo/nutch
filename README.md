# Apache Nutch — модульный фреймворк для построения поисковых систем, написанный на языке Java таких как yandex или google

На базе Nutch 2.0, запущенного поверх 34-узлового Hadoop-кластера, построен поисковый сервис компании Kalooga, в индексе которого находится более миллиарда страниц. 

![alt text](https://cf.ppt-online.org/files1/slide/i/ICJo6extfvTVQnc0lik45BsqK2NyG8drHzOmaPjE7/slide-34.jpg)


# Архитектура [nutch] & Реверс инжениринг

https://drive.google.com/drive/folders/13V9bx41gtxNxtYkfGE3p01UO0sqMKQ5G

![alt text](https://sites.google.com/site/nutch1936/_/rsrc/1427176500763/home/introduction/Nutch_Overview.png)

Apache Nutch — модульный фреймворк для построения поисковых систем, написанный на языке Java и основанный на технологиях Lucene, Solr, Tika, Hadoop и Gora, адаптированных для специфики поиска в интернете (например, поддерживается crawler, база ссылочной связи, парсинг HTML и других форматов). Архитектура Nutch позволяет разработчикам создавать плагины для обработки нового медиа-контента, получение данных через нестандартные каналы для формирования типовых запросов или организации поискового кластера.
Система предоставляет средства для построения высокомасштабных систем индексации, отвлеченных от типа хранилища, что позволяет использовать такие хранилища для больших объемов данных, как Apache Accumulo, Apache Avro, Apache Cassandra, Apache HBase и HDFS, так и SQL-базы и размещение в памяти NoSQL БД.
На базе Nutch 2.0, запущенного поверх 34-узлового Hadoop-кластера, построен поисковый сервис компании Kalooga, в индексе которого находится более миллиарда страниц[1].

# Apache Nutch README
===================

<img src="http://nutch.apache.org/assets/img/nutch_logo_tm.png" align="right" width="300" />

For the latest information about Nutch, please visit our website at:

   http://nutch.apache.org

and our wiki, at:

   http://wiki.apache.org/nutch/

To get started using Nutch read Tutorial:

   http://wiki.apache.org/nutch/NutchTutorial
   
Contributing
============
To contribute a patch, follow these instructions (note that installing
[Hub](http://hub.github.com) is not strictly required, but is recommended).

```
0. Download and install hub.github.com
1. File JIRA issue for your fix at https://issues.apache.org/jira/browse/NUTCH
- you will get issue id NUTCH-xxx where xxx is the issue ID.
2. git clone http://github.com/apache/nutch.git 
3. cd nutch
4. git checkout -b NUTCH-xxx
5. edit files (please try and include a test case if possible)
6. git status (make sure it shows what files you expected to edit)
7. Make sure that your code complies with the [Nutch codeformatting template](http://svn.apache.org/repos/asf/nutch/branches/2.x/eclipse-codeformat.xml), which is basially two space indents
8. git add <files>
9. git commit -m “fix for NUTCH-xxx contributed by <your username>”
10. git fork
11. git push -u <your git username> NUTCH-xxx
12. git pull-request
```
   
Export Control
==============
This distribution includes cryptographic software.  The country in which you 
currently reside may have restrictions on the import, possession, use, and/or 
re-export to another country, of encryption software.  BEFORE using any encryption 
software, please check your country's laws, regulations and policies concerning the
import, possession, or use, and re-export of encryption software, to see if this is 
permitted.  See <http://www.wassenaar.org/> for more information. 

The U.S. Government Department of Commerce, Bureau of Industry and Security (BIS), has 
classified this software as Export Commodity Control Number (ECCN) 5D002.C.1, which 
includes information security software using or performing cryptographic functions with 
asymmetric algorithms.  The form and manner of this Apache Software Foundation 
distribution makes it eligible for export under the License Exception ENC Technology 
Software Unrestricted (TSU) exception (see the BIS Export Administration Regulations, 
Section 740.13) for both object code and source code.

The following provides more details on the included cryptographic software:

Apache Nutch uses the PDFBox API in its parse-tika plugin for extracting textual content 
and metadata from encrypted PDF files. See http://pdfbox.apache.org for more 
details on PDFBox.
