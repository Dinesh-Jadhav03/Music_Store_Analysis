# 🎵 Music Store Analysis (SQL Server)

## 📌 Overview
This project focuses on analyzing the **music store database** using **SQL Server** to extract insights related to **sales, customer behavior, and track popularity**.

## 🗄️ Database Schema
The database consists of multiple tables:

### 🎼 Music Data
- **Artist** (`ArtistId`, `Name`)
- **Album** (`AlbumId`, `Title`, `ArtistId`)
- **Track** (`TrackId`, `Name`, `AlbumId`, `MediaTypeId`, `GenreId`, `Composer`, `Milliseconds`, `Bytes`, `UnitPrice`)
- **Genre** (`GenreId`, `Name`)
- **MediaType** (`MediaTypeId`, `Name`)

### 📋 Playlists
- **Playlist** (`PlaylistId`, `Name`)
- **PlaylistTrack** (`PlaylistId`, `TrackId`)

### 👥 Customers & Employees
- **Customer** (`CustomerId`, `FirstName`, `LastName`, `Company`, `Address`, `City`, `State`, `Country`, `PostalCode`, `Phone`, `Fax`, `Email`, `SupportRepId`)
- **Employee** (`EmployeeId`, `LastName`, `FirstName`, `Title`, `ReportsTo`, `BirthDate`, `HireDate`, `Address`, `City`, `State`, `Country`, `PostalCode`, `Phone`, `Fax`, `Email`)

### 🧾 Sales & Invoices
- **Invoice** (`InvoiceId`, `CustomerId`, `InvoiceDate`, `BillingAddress`, `BillingCity`, `BillingState`, `BillingCountry`, `BillingPostalCode`, `Total`)
- **InvoiceLine** (`InvoiceLineId`, `InvoiceId`, `TrackId`, `UnitPrice`, `Quantity`)

## 🎯 SQL Server Analysis Goals
- Identify **top-selling** tracks, albums, and artists.
- Analyze **customer purchasing trends**.
- Find **highest revenue-generating genres**.
- Determine **monthly and yearly sales trends**.
- Evaluate **employee contributions** to sales.

## 🛠️ SQL Server Queries Used
- **Aggregations** (`SUM()`, `COUNT()`, `AVG()`)
- **Joins** (`INNER JOIN`, `LEFT JOIN`)
- **Filtering** (`WHERE`, `HAVING`)
- **Grouping** (`GROUP BY`)
- **Sorting** (`ORDER BY`,`Limit`)
- **Common Table Expressions (CTEs)** (`WITH ... AS`)
- **Window Functions** (`RANK()`, `DENSE_RANK()`, `ROW_NUMBER()`, `OVER()`)
- **Indexes** (`CREATE INDEX`)
- **Performance Optimization** (Query execution plans, indexing strategies)


## 🚀 How to Use
1. **Connect to SQL Server** using SQL Server Management Studio (SSMS) or Azure Data Studio.
2. **Import the database schema** if not already available.
3. **Run SQL queries** to extract and analyze data.
4. **Optimize queries** for better performance and insights.

## 📄 License
This project is open-source and available for educational and analytical purposes.

---

💡 *Feel free to contribute or suggest improvements!*



