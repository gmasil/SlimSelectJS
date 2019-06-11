# SlimSelectJS
This is a redistribution of the slimselectjs by [Brian Voelker](https://github.com/brianvoe) for maven based projects.  
You can find his GitHub repo under [https://github.com/brianvoe/slim-select](https://github.com/brianvoe/slim-select).  
See [http://slimselectjs.com/](http://slimselectjs.com/) for more information.

## Usage
Maven dependency:

    <dependency>
	   <groupId>de.gmasil.thirdparty</groupId>
      <artifactId>slimselectjs</artifactId>
      <version>1.20.0</version>
    </dependency>

Add the repository to your pom or settings:

    <repositories>
      <repository>
        <id>gmasil-nexus</id>
        <url>https://nexus.gmasil.de/repository/maven-releases/</url>
      </repository>
    </repositories>

In Spring based projects you might want to add the resource location:

```java
@Configuration
public class SlimselectConfig implements WebMvcConfigurer {
  @Override
  public void addResourceHandlers(ResourceHandlerRegistry registry) {
    registry.addResourceHandler("/slimselectjs/**").addResourceLocations("classpath:/slimselectjs/1.20.0/");
  }
}
```

## License
```
MIT License

Copyright (c) 2017 Brian Voelker

Permission is hereby granted, free of charge, to any person obtaining a copy  
of this software and associated documentation files (the "Software"), to deal  
in the Software without restriction, including without limitation the rights  
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell  
copies of the Software, and to permit persons to whom the Software is  
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all  
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR  
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,  
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE  
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER  
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,  
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE  
SOFTWARE.
```
