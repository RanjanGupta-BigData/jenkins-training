If you are getting issues with the java compatibiliy due to upgrade from java7 to Java8.
The issue will mainly come if you are using other softwares that use Java 7.

Try to install  java-1.8.0-openjdk-devel
This will install Javac as well

    bash-4.2# yum install java-1.8.0-openjdk-devel

Then go on for selecting *javac* from java8  as your default java compiler by using alternatives command.
Repeat the same, if you have to, for Java as well  :
 
   [root@ip-172-31-17-118 ec2-user]# alternatives --config javac

There are 2 programs which provide 'javac'.

      Selection    Command
    -----------------------------------------------
    *  1           /usr/lib/jvm/java-1.7.0-openjdk.x86_64/bin/javac
     + 2           /usr/lib/jvm/java-1.8.0-openjdk.x86_64/bin/javac

Enter to keep the current selection[+], or type selection number: 2

 
