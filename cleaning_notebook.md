# Cleaning Decisions

## Columns in the Feature Set

| Column Kept | Reason |
| --- | --- |
|  PClass | The class that the passengers were in related to their position on the ship anf how likely the crew would be to help them |
| Sex | Women were typically given preference for lifeboats |
| Age | Split into children, adults, and elderly |
| SibSp | If a person had a sibling or spouse, they might be more likely to try and save that person |
| Parch | A parent would likely try to give up their spot for a child |

## Columns Excluded from the Feature Set

| Column Excluded | Reason |
| --- | --- |
| PassengerId | This is just a number to keep track of passengers within the dataset |
| Name | Too unique to split |
| Ticket, fare, cabin | Same reasoning for all of these, they correlate highly with passenger class which is fully filled, whereas some of these are not |
| Embarked | This is probably not a factor that would have been apparent when deciding who went into lifeboats |

## Splitting the Ages

The ages were split into 3 categories, children < 18, adults between 18 and 65, and elderly >= 65.