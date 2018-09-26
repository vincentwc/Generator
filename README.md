# Generator
first commit
快速使用逆向工程
此项目用于快捷生成java文件
只需配置相应的数据库就行

###    第一步：

       在src/generator.properties文件下配置basepackage属性：表示生成文件的目录
       在src/generator.properties文件下配置数据库的属性,以oracle为例，配置文件中也有其他类型数据库的连接配置
        jdbc.username=
        jdbc.password=
        jdbc.url=jdbc:oracle:thin:@localhost:1521:orcl
        jdbc.driver=oracle.jdbc.driver.OracleDriver
       在outRoot=C:/generator-output
       注意：该目录最好是没有存储文件的目录，逆向工程会先删除该目录然后在创建
       
###    第二步：

       在src/GeneratorMain.java的main方法中写入要生成的表名称，以DEMO表为例
      g.generateByTable("DEMO");
      
  
 ###   运行main方法即可
