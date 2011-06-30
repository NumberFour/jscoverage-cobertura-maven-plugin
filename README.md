#jscoverage to Cobertura Maven Plugin

This plugin converts jscoverage's JSON output into the Cobertura XML format. It is configured as follows:
    
    <build>
    ....
    <plugin>
      <groupId>de.mytoys.maven.plugins</groupId>
      <artifactId>jscoverage-cobertura-maven-plugin</artifactId>
      <groupId>eu.numberfour.maven.plugins</groupId>
      <version>1.2.0</version>
      <executions>
        <execution>
          <goals>
           <goal>transform</goal>
          </goals>
          <phase>process-resources</phase>
        </execution>
      </executions>
    </plugin>
    ...
    </build>

Alternatively you can run it from the command line with the following line:

    mvn eu.numberfour.maven.plugins:jscoverage-cobertura-maven-plugin:transform

The complete Mojo documentation is available here: http://numberfour.github.com/jscoverage-cobertura-maven-plugin/transform-mojo.html
