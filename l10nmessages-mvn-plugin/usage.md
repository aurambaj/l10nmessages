```xml
<plugin>
  <groupId>com.pinterest.l10nmessages</groupId>
  <artifactId>l10nmessages-mvn-plugin</artifactId>
  <version>1.0.4</version>
  <dependencies>
    <dependency>
      <groupId>com.ibm.icu</groupId>
      <artifactId>icu4j</artifactId>
      <version>72.1</version>
    </dependency>
  </dependencies>
  <executions>
    <execution>
      <goals>
        <goal>generate</goal>
      </goals>
    </execution>
  </executions>
  <configuration>
    <l10nPropertiesList>
      <l10nProperties>
        <baseName>com.pinterest.l10nmessages.Message</baseName>
        <onDuplicatedKeys>ACCEPT_IF_SAME</onDuplicatedKeys>
        <messageFormatValidationTargets>ROOT</messageFormatValidationTargets>
      </l10nProperties>
    </l10nPropertiesList>
  </configuration>
</plugin>
```