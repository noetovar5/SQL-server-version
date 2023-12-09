# SQL-server-version                 <img align="right" src="https://visitor-badge.laobi.icu/badge?page_id=noetovar5.SQL-server-version"/>       
Find out SQL server version



Find out SQL server version
SELECT SERVERPROPERTY('productversion') as Version, SERVERPROPERTY ('productlevel') as Level, SERVERPROPERTY ('edition') as Edition, @@servername 'Server Name', substring(@@version,1,charindex('-',@@version)-1) +convert(varchar(100),SERVERPROPERTY('edition'))+ ' '+ +convert(varchar(100),SERVERPROPERTY('productlevel'))'Server Version'
