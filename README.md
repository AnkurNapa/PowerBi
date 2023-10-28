# PowerBi
##DAX Calendar 
DAX expression: 
Date = ADDCOLUMNS ( CALENDAR (DATE(2000,1,1), DATE(2025,12,31)), "DateAsInteger", FORMAT ( [Date], "YYYYMMDD" ), "Year", YEAR ( [Date] ), "MonthNo", FORMAT ( [Date], "MM" ), "YearMonthNo", FORMAT ( [Date], "YYYY/MM" ), "YearMonth", FORMAT ( [Date], "YYYY/mmm" ), "MonthShort", FORMAT ( [Date], "mmm" ), "MonthLong", FORMAT ( [Date], "mmmm" ), "WeekNo", WEEKDAY ( [Date] ), "WeekDay", FORMAT ( [Date], "dddd" ), "WeekDayShort", FORMAT ( [Date], "dddd" ), "Quarter", "Q" & FORMAT ( [Date], "Q" ), "YearQuarter", FORMAT ( [Date], "YYYY" ) & "/Q" & FORMAT ( [Date], "Q" )
