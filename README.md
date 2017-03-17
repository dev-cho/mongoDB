<h2>몽고 DB Centos7 설치</h2>
<a href="https://robomongo.org/download">https://robomongo.org/ 참고</a>

<p>* yum install vim</p>

<div>
	<h2> 1) Configure the package management system (yum) </h2>
	<p># Create a /etc/yum.repos.d/mongodb-org-3.4.repo file so that you can install MongoDB directly, using yum </p>
</div>
<p>vim /etc/yum.repos.d/mongodb.repo</p>
<div>
	<h4>Centos7 64bit</h4>
	<p># [mongodb-org-3.4] </p>
	<p># name=MongoDB Repository</p>
	<p># baseurl=https://repo.mongodb.org/yum/redhat/$releasever/mongodb-org/3.4/x86_64/</p>
	<p># gpgcheck=1</p>
	<p># enabled=1</p>
	<p># gpgkey=https://www.mongodb.org/static/pgp/server-3.4.asc</p>
</div>
<div>
	<h4>Centos7 32bit</h4>
	<p># [mongodb-org-2.6]</p>
	<p># name=MongoDB Repository</p>
	<p># baseurl=http://downloads-distro.mongodb.org/repo/redhat/os/i686/</p>
	<p># gpgcheck=0</p>
	<p># enabled=1</p>
</div>
<div>
	<h2> 2) Install MongoDB </h2>
	<p># 2-1 yum update</p>
	<p># 2-2 yum install mongodb-org mongodb-org-server</p>
</div>
