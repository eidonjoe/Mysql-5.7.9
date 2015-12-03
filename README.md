# Mysql-5.7.9
mac mysql install 

##原料mac OS X 10.11 homebrew
1.安装mysql
<pre><code>brew install mysql</code></pre>
等待安装期间会出现
<pre><code>
==> Downloading https://homebrew.bintray.com/bottles/mysql-5.7.9.el_capitan.bottle.1.tar.gz
######################################################################## 100.0%
==> Pouring mysql-5.7.9.el_capitan.bottle.1.tar.gz
==> /usr/local/Cellar/mysql/5.7.9/bin/mysqld --initialize-insecure --user=zhd --basedir=/usr/local/Cellar/mysql/5.7.9 --datadir=/usr/local/var/mysql --tmpdir=/tmp
==> Caveats
</code></pre>
安装成功后会提示
<pre><code>
We've installed your MySQL database without a root password. To secure it run:
    mysql_secure_installation

To connect run:
    mysql -uroot

To reload mysql after an upgrade:
  launchctl unload ~/Library/LaunchAgents/homebrew.mxcl.mysql.plist
  launchctl load ~/Library/LaunchAgents/homebrew.mxcl.mysql.plist
Or, if you don't want/need launchctl, you can just run:
  mysql.server start
==> Summary
🍺  /usr/local/Cellar/mysql/5.7.9: 12629 files, 464M
</code></pre>
**`注意:`**执行`mysql_secure_installation`是开启mysql的安全机制,也就是在这个时候,可以给你的`root`用户设置密码,如果没有这一步,你的mysql是无法正常工作的,后续会有一些提示设置,按照提示执行即可.
