--1
SELECT ProductName, QuantityPerUnit
FROM Products;

--2
SELECT ProductID, ProductName
FROM Products
WHERE Discontinued = 'FALSE';

--3
SELECT ProductID, ProductName
FROM Products
WHERE Discontinued = 'TRUE';

--4
SELECT ProductName, UnitPrice
FROM Products
ORDER BY UnitPrice DESC;

--5
SELECT ProductID ,ProductName, UnitPrice
FROM Products
WHERE Discontinued = 'FALSE' AND UnitPrice < 20
ORDER BY UnitPrice;

--6
SELECT ProductID ,ProductName, UnitPrice
FROM Products
WHERE (Discontinued = 'FALSE') AND (UnitPrice BETWEEN 15 AND 25)
ORDER BY UnitPrice;

--7
SELECT ProductName, UnitPrice
FROM Products 
WHERE UnitPrice > (SELECT AVG(UnitPrice) FROM Products)
ORDER BY UnitPrice;

--8
SELECT TOP 10 ProductName, UnitPrice
FROM Products 
ORDER BY UnitPrice DESC;

--9
SELECT Discontinued, COUNT(ProductID) AS products
FROM Products
GROUP BY Discontinued;

--10
SELECT ProductName AS ProductToBuy, UnitsOnOrder, UnitsInStock
FROM Products 
WHERE UnitsInStock < UnitsOnOrder AND Discontinued = 'FALSE';
