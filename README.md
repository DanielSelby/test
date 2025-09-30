# Project: Global Military Fire Power
-----

## Table Of Contents
1. [Project overview](#Project-overview)
2. [Business questions](#Business-questions)
3. [Conclusion](#Conclusion)

[Check this link](https://fp20analytics.com/datasets/)

## Project overview

## Business questions

## Objectives and deliverables

## Data source
WHere did you get the datset?  
How many rows?  
How many columns?  
* _Employee_Id_:	Unique employee identifier
* _Full_Name_:	Employee full name (synthetic)
* Gender	Employee gender (M/F/Other)
* Age	Employee age in years  
Education_Level	Highest education level achieved  
Hire_Date	Date when employee was hired (dd/mm/yyyy)  
Exit_Date	Date when employee left (dd/mm/yyyy, blank if active)  
Department	Business department/division  
Job_Role	Specific job position/title  
Job_Level	Seniority level (Entry/Associate/Supervisor/Manager/Executive)  
Employment_Type	Employment classification (Full-time/Part-time/Seasonal/Contractor)
Store_Location	City/region where employee works
Store_Location_Latitude	Data field - see sheet for values
Store_Location_Longitude	Data field - see sheet for values
Store_Id	Store identifier
Manager_Id	Direct manager employee ID
Base_Salary_Annual	Annual base salary in currency units


## Data cleaning 
Preview the data.
What did you do?

```python
print("Data Analytics is sweet!")
```

```sql
SELECT
  Daniel,
  Cindy,
  Emmanuel,
  Nana,
  Euginia
FROM Blossom_Academy
WHERE Job_role = TRUE
GROUP BY Industry
```
```sql
SELECT 
	c.name,
    w.wishes ->> 'first_choice' AS primary_wish,
    w.wishes ->> 'second_choice' AS secondary_wish,
    (w.wishes -> 'colors'->> 0) AS favorite_color,
    json_array_length(w.wishes -> 'colors') AS color_count,
	CASE
		WHEN t1.difficulty_to_make = 1 THEN 'Simple Gift'
		WHEN t1.difficulty_to_make = 2 THEN 'Moderate Gift'
		WHEN t1.difficulty_to_make >= 3 THEN 'Complex Gift'
	END AS gift_complexity,
	CASE
		WHEN t1.category = 'outdoor' THEN 'Outside Workshop'
		WHEN t1.category = 'educational' THEN 'Learning Workshop'
		ELSE 'General Workshop'
	END AS assigned_workshop
FROM children AS c
LEFT JOIN wish_lists AS w
	ON c.child_id = w.child_id
LEFT JOIN toy_catalogue AS t1
	ON (w.wishes ->> 'first_choice') = t1.toy_name
LEFT JOIN toy_catalogue AS t2
	ON (w.wishes ->> 'first_choice') = t2.toy_name
ORDER BY c.name ASC
LIMIT 5;
;
```

> [!NOTE]
> Your GitHub is your portfolio

> [!IMPORTANT]
> Posting on LinkedIn will open doors for you.

> [!TIP]
> 1. Post at least three times a week go gain visibility.
> 2. Comment on other people's posts

> [!WARNING]
> Do not compare yourself to other people.

## Data Modeling


## Data analysis


## Data visualization
|Wireframing|
|:------:|

![Wireframing](https://github.com/DanielSelby/test/blob/main/Picture1.png)

|Wireframing|
|:------:|


<figure>
  <img src="https://github.com/DanielSelby/test/blob/main/Picture1.png" width=100% height=100% alt="alt text">
  <figcaption>Figure: Wireframing</figcaption>
</figure>

## Insights 
## 𝐓𝐞𝐬𝐭 𝐭𝐡𝐢𝐬 𝐭𝐞𝐱𝐭.

## Recommendations

## Conclusion





