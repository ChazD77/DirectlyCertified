SELECT LastName, FirstName, Mid, StatusType, BirthDate

FROM Customers

WHERE StatusType = 'directly certified'

GROUP BY LastName, FirstName, Mid, BirthDate, StatusType

HAVING COUNT (*) >1
