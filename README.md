# Housing_Project
Imported Data set about Housing sales from an .xlsx file into Microsoft SQL Studio Management in order to perform data scrubbing. The objectives for this included:
  - Standardize the data format (completed by changing data type to remove the seconds measurement)
  - Populate property address data that had null records (completed by matching identical records with 1 record missing an address, then adding the address using a SELF      JOIN)
  - Breaking out complete addresses into individual columns of street address, city, and state (completed in 2 different ways: 1) using SUBSTRING and indicated the stop      and start points with CHARINDEX 2) using PARSENAME)
  - Changing 4 responses of Y, N, Yes, and No into only Yes and No in the "Sold as vacant" field (completed by CASE statement)
  - Removed duplicates (completed using ROW_NUMBER to identify duplicate rows, then utilizing a CTE to remove duplicate rows
  - Delete Unused Columns (completed by ALTER TABLE - DROP statement)
