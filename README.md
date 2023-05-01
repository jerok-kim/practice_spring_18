## [최주호] 스프링 강의 - 테이블 연관 관계와 Lazy, Eager

### 연관관계

Hibernate는 객체-관계 매핑(Object-Relational Mapping, ORM)을 지원하여, 객체 지향 프로그래밍에서 사용되는 객체와 관계형 데이터베이스의 테이블 간의 연관관계를 매핑할 수 있다.

Hibernate에서는 다음과 같은 연관관계를 지원한다.

1. 일대일(One-to-One) 연관관계: 두 개의 엔티티 간에 하나의 관계만 존재하는 경우
2. 일대다(One-to-Many) 연관관계: 하나의 엔티티가 다른 엔티티 여러 개와 연관된 경우
3. 다대일(Many-to-One) 연관관계: 여러 개의 엔티티가 하나의 엔티티와 연관된 경우
4. 다대다(Many-to-Many) 연관관계: 연관관계 여러 개의 엔티티가 다른 여러 개의 엔티티와 연관된 경우

연관관계의 주인은 `mappedBy` 속성으로 설정할 수 있다.

FK는 N쪽에 붙이면 된다. N쪽이 항상 연관관계의 주인이다.