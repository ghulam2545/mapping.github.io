JPA mapping

### Unidirectional relationship
[one to one mapping](pages/uni_one_to_one.md)

[one to many mapping](pages/uni_one_to_many.md)

[many to one mapping](pages/uni_many_to_one.md)

[many to many mapping](pages/uni_many_to_many.md)

### Bidirectional relationship
[one to one mapping](pages/bi_one_to_one.md)

[one to many mapping](pages/bi_one_to_many.md)

[many to one mapping](pages/bi_many_to_one.md)

[many to many mapping](pages/bi_many_to_many.md)


Points:
- In unidirectional mapping only one class will have reference of other
- In Bidirectional mapping both class will be having reference to each other

- In one-to-one OR many-to-many either side can be
    1. parent entity
    2. Can have foreign key
    3. owns the relationship
- In one-to-many OR many-to-one, many side 
    1. will be parent entity
    2. will be having foreign key
    3. and owns relationship

- @JoinColumn, @JoinTable are optional