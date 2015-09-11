`wget https://dl.bintray.com/jfrog/artifactory-pro/org/artifactory/pro/jfrog-artifactory-pro/4.1.0/jfrog-artifactory-pro-4.1.0.zip
`unzip jfrog-artifactory-pro-4.1.0.zip
`
`git clone https://github.com/alexivenin/artifactory-debian
`cp -rv artifactory-debian/debian/ artifactory-pro-4.1.0/
`cd artifactory-pro-4.1.0
`
`# download latest version of postgresql jdbc driver from https://jdbc.postgresql.org/download.html#supported
`wget https://jdbc.postgresql.org/download/postgresql-9.3-1103.jdbc4.jar
`mv postgresql-9.3-1103.jdbc4.jar tomcat/lib/
`
`debuild -us -uc -b
