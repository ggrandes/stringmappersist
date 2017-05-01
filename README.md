# stringmappersist

Persistence of Map using same format as java.util.Properties (load/store), but ordered maintained. Open Source Java project under GNU General Public License, version 2, with the Classpath Exception.

### Current Stable Version is [1.0.0](https://search.maven.org/#search|ga|1|g%3Aorg.javastack%20a%3Astringmappersist)

---

## DOC

#### Usage Example

```java
import org.javastack.stringmappersist.StringMapPersist;

public class Example {
	public static void main(final String[] args) throws Throwable {
		Map<String, String> map = new LinkedHashMap<String, String>();
		StringMapPersist p = new StringMapPersist(map);
		map.put("state", "awake");
		map.put("msg", "Hi user, how are you?");
		p.store(System.out, "DATA");
	}
}
```

##### The Result:

	state=awake
	msg=Hi user, how are you?

---

## MAVEN

Add the dependency to your pom.xml:

    <dependency>
        <groupId>org.javastack</groupId>
        <artifactId>stringmappersist</artifactId>
        <version>1.0.0</version>
    </dependency>

---
Inspired in [Java Properties](http://docs.oracle.com/javase/7/docs/api/java/util/Properties.html), this code is for compatibility format.
