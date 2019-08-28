### siren4j
---
https://github.com/eserating/siren4j

```java
@Siren4JEntity(name = "video", uri = "/videos/{id}")
public class Video extends BaseResource {
 
  private String id;
  private String name;
  private String description;
  private String genre;
  private Rating rating;
  @Siren4JSubEntity(uri = "/video/{parent.id}/reviews", embeddedLink = true)
  private CollectionResouce<Review> reviews;
  
  public String getId() {return id;}
  public void setId(String id) {this.id = id};
  public String getName() {return name;}
  public void getDescription() {return description;}
  
  
  public enum Rating {G, PG, PG13, R, NR, X}
}


```

```
```

```
```


