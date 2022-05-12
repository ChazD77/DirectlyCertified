SELECT LastName, FirstName, Mid, StatusType, BirthDate

FROM customers

WHERE StatusType = 'directly certified'

GROUP BY LastName, FirstName, Mid, BirthDate, StatusType

HAVING COUNT (*) >1
