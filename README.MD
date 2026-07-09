-- Find the sales which are above from the average sales


select * from samplesuperstore
where sales > (select AVG(sales)  from samplesuperstore )
limit 5;
|Ship Mode|Segment|Country|City|State|Postal Code|Region|Category|Sub-Category|Sales|Quantity|Discount|Profit|
|---------|-------|-------|----|-----|-----------|------|--------|------------|-----|--------|--------|------|
|Second Class|Consumer|United States|Henderson|Kentucky|42420|South|Furniture|Bookcases|261.96|2|0.0|41.9136|
|Second Class|Consumer|United States|Henderson|Kentucky|42420|South|Furniture|Chairs|731.94|3|0.0|219.582|
|Standard Class|Consumer|United States|Fort Lauderdale|Florida|33311|South|Furniture|Tables|957.5775|5|0.45|-383.031|
|Standard Class|Consumer|United States|Los Angeles|California|90032|West|Technology|Phones|907.152|6|0.2|90.7152|
|Standard Class|Consumer|United States|Los Angeles|California|90032|West|Furniture|Tables|1706.184|9|0.2|85.3092|

