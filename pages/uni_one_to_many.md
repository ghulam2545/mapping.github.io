![image](../images/image_3.png)

```java
@Entity(name = "book")
public class Book {

    @Id
    @GeneratedValue
    private Long book_id;
    private String title;
    private Integer price;
    // ...

    @OneToMany
    @JoinColumn(name = "book_id_fk", referencedColumnName = "book_id")
    private List<Review> reviews = new ArrayList<>();
}
```

```java
@Entity(name = "review")
public class Review {

    @Id
    @GeneratedValue
    private Long review_id;
    private String content;
    // ...
}
```