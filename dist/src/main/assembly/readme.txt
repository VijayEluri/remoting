Seam Remoting 3.0.0 Beta 2
==========================

Seam Remoting is an AJAX remoting API for CDI-based applications.


Contents of distribution
========================

doc/

  API Docs and reference guide.
  
examples/

  Seam Remoting Examples
  
lib/

  Seam Remoting jar files
  
Licensing
=========

This distribution, as a whole, is licensed under the terms of the GNU Lesser General Public License
(LGPL) Version 2.1, the text of which is contained in the file lgpl.txt.

Seam Remoting URLs
==================

Seam Framework Home Page:      http://www.seamframework.org
Downloads:                     http://www.seamframework.org/Download/SeamDownloads
Forums:                        http://www.seamframework.org/Community/SeamUsers
Source Code:                   git://github.com/seam/js-remoting.git
Issue Tracking:                http://jira.jboss.org/jira/browse/SEAMREMOTING

Release Notes
=============
Version 3.0.0 Beta 2
--------------------
* Added new feature - bean validation
* Updated to use Seam Solder 

Version 3.0.0 Beta 1
--------------------
First beta release of Seam Remoting 3.x, ported from Seam 2.x to CDI.

* Added new feature - Model API
* Simplified JavaScript stubs for server-side beans
* Added option to compress remote.js - add ?compress=true to URL
* Experimental JMS support (that was present in Seam 2.x) has been removed - this feature will be
  provided at a later date by a unified AJAX event bus.
* Support for batch requests has been removed

* If using Maven, some artifacts may only be available in the JBoss Repository. To allow Seam Remoting to correctly function, add the JBoss Repository to Maven. Edit your ~/.m2/settings.xml, and add the following entry:

      <profile>
         <id>jboss.repository</id>
         <activation>
            <activeByDefault>true</activeByDefault>
         </activation>
         <repositories>
            <repository>
               <id>repository.jboss.org</id>
               <url>http://repository.jboss.org/maven2</url>
               <releases>
                  <enabled>true</enabled>
               </releases>
               <snapshots>
                  <enabled>false</enabled>
               </snapshots>
            </repository>
         </repositories>
      </profile>
