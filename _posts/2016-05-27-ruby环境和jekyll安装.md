---
layout: post
title: ruby 和 jekyll 本地环境搭建
data: 2016-05-27 
categories: ruby
---
# 1、ruby 环境安装 

use rvm to manager ruby

#### install rvm
{% highlight ruby %}
gpg --keyserver hkp://keys.gnupg.net --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3
\curl -sSL https://get.rvm.io | ruby -s stable
source /home/james/.rvm/scripts/rvm
{% endhighlight ruby %}

#### install ruby
{% highlight ruby %}
rvm install ruby-2.3.1
rvm 2.3.1 --default
{% endhighlight ruby %}

#### 更新gem库和gem版本
{% highlight ruby %}
gem -v
gem source -r https://rubygems.org/
gem source -a http://gems.ruby-china.org/
gem source -l
gem update --system
{% endhighlight ruby %}

#### install rails
{% highlight ruby %}
gem install rails
{% endhighlight ruby %}

# 2、nodejs 安装

#### download nodejs

	wget https://nodejs.org/dist/v4.4.5/node-v4.4.5.tar.gz

####  解压缩 tar.gz包

	tar -zxvf node-v4.4.5.targz

####  安装

{% highlight ruby %}
	cd node-v4.4.5-linux-x64/
	./configure --prefix =/usr
	make
	sudo make install
{% endhighlight ruby %}



# 3、jekyll 安装

        gem install jekyll

# 4、启动jekyll 本地

        jekyll server

浏览器中打开以下地址  http://localhost:4000


