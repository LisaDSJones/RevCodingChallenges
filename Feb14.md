# Java

```java
public static String actualMemorySize (String startSize) {
	float answer = Math.round( Float.parseFloat(startSize.substring(0, startSize.length()-2))*93)/100;
	String bytes = startSize.substring(startSize.length()-2);
	
	if (answer < 1) { // convert to mb notation
		answer = Math.round(answer*1024);
		bytes = "MB";
	}

	return answer + bytes;
}
```
