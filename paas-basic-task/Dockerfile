FROM centos:7	FROM centos:7
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone	RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone
RUN yum -y install wget	RUN yum -y install wget
RUN yum -y install java	RUN yum -y install java
RUN yum -y install httpd php php-gd	RUN yum -y install httpd php php-gd
RUN yum -y install initscripts	RUN yum -y install initscripts
RUN yum -y install gcc openssl-devel bzip2-devel	RUN yum -y install gcc openssl-devel bzip2-devel
RUN yum -y install python	RUN yum -y install python
RUN yum -y install make gcc-c++ 	RUN yum -y install make gcc-c++ 


RUN curl --silent --location https://rpm.nodesource.com/setup_8.x | bash -	RUN curl --silent --location https://rpm.nodesource.com/setup_8.x | bash -
RUN yum -y install nodejs	RUN yum -y install nodejs

RUN curl https://packages.microsoft.com/config/rhel/7/prod.repo > /etc/yum.repos.d/microsoft.repo 	
RUN yum -y install powershell	
RUN wget https://github.com/PowerShell/PowerShell/releases/download/v6.0.0-alpha.9/powershell-6.0.0_alpha.9-1.el7.centos.x86_64.rpm	
RUN yum install -y libunwind libicu	
RUN yum -y remove powershell	
RUN rpm -ivh powershell-6.0.0_alpha.9-1.el7.centos.x86_64.rpm
