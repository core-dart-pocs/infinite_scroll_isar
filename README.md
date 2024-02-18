infinite_scroll_pagination and isar examples

### Tests
#### Null -> 1
Given an infinite scroll paginated view watching an empty query
When an item is added to the query scope
Then the item's element should be findable on the screen


#### Remove item
Given an infinite scroll paginated view watching a query with 2 pages overflow (3 pages total)
When the view is scrolled to the second page
And an item in the first page result set is removed
Then the item's element should not exist
