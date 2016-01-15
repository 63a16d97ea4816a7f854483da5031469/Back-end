##Failed to execute goal org.apache.maven.plugins:maven-war-plugin:2.2:war


mvn install issue:

[ERROR] Failed to execute goal org.apache.maven.plugins:maven-war-plugin:2.2:war
 (default-war) on project Que: Error assembling WAR: webxml attribute is require
d (or pre-existing WEB-INF/web.xml if executing in update mode) -> [Help 1]

http://stackoverflow.com/questions/5351948/webxml-attribute-is-required-error-in-maven

It would be helpful if you can provide a code snippet of your maven-war-plugin. Looks like the web.xml is at right place, still you can try and give the location explicitly

	<plugin>            
	  <groupId>org.apache.maven.plugins</groupId>
	  <artifactId>maven-war-plugin</artifactId>
	  <configuration>
	    <webXml>src\main\webapp\WEB-INF\web.xml</webXml>        
	  </configuration>
	</plugin>