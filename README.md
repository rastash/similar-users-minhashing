# similar-users-minhashing
Given a set of items, and baskets of these items consumed by users, determine similar users.

## Problem Definition
Given a large set of items, and baskets of these items representing
consumption from users, identify similar users. The total number of
items and the total number of users can be large. However, the number
of items appearing in any one basket is typically small.

## Input
It is most efficient to represent the input as a matrix, where each
row corresponds to a user, and each column represents an item. When
consumption is indicated by a binary variable (read the article or
not, clicked on the link or not), then a bit-vector is the most
efficient way to represent this matrix. We use the bitarray class (see
(link)[https://pypi.python.org/pypi/bitarray/0.8.1] for more details).