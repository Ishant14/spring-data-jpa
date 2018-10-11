## Spring-data-jpa

Each of these defines its own functionality:

**CrudRepository** provides CRUD functions, 
**PagingAndSortingRepository** provides methods to do pagination and sort records, 
**JpaRepository** provides JPA related methods such as flushing the persistence context and delete records in a batch

> And so, because of this inheritance relationship, the JpaRepository contains the full API of CrudRepository and 
PagingAndSortingRepository.

When we don’t need the full functionality provided by JpaRepository and PagingAndSortingRepository, 
we can simply use the CrudRepository.
