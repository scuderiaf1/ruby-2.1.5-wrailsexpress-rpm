# ruby-2.1.x-wrailsexpress-rpm

### How to install

### Autoconf 
* version 2.67 or higher is required. Check it autoconf -V 

    cd /tmp
    wget ftp://ftp.pbone.net/mirror/ftp5.gwdg.de/pub/opensuse/repositories/home:/monkeyiq:/centos6updates/CentOS_CentOS-6/noarch/autoconf-2.69-12.2.noarch.rpm
    yum install autoconf-2.69-12.2.noarch.rpm


#### RHEL/CentOS 6

    yum -y install rpmdevtools glibc-devel readline-devel libyaml-devel ncurses-devel gdbm-devel tcl-devel openssl-devel db4-devel libffi-devel make gcc unzip byacc
    rpmdev-setuptree
    cd ~/rpmbuild/SOURCES
    wget wget http://ftp.ruby-lang.org/pub/ruby/2.1/ruby-2.1.5.tar.gz
    cd ~/rpmbuild/SPECS
    wget https://raw.github.com/scuderiaf1/ruby-2.1.x-wrailsexpress/master/ruby21-railsexpress.spec
    QA_RPATHS=$[ 0x0001|0x0010 ]  rpmbuild -bb ruby21-railsexpress.spec


### So far works with


* CentOS 6.6 x86_64
