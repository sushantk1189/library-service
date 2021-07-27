********************Book Library Management System***********************
Library Management System is used to fetch book details,
search books on basis of Id , 
delete books from details whichever not required
and we can import book details from csv file easily

below are api details  providing with request body
1.POST: http://localhost:8282/api/v1/library/save
{
	"bookDetails":{
		"id":1,
		"isbn":"1900001",			
		"title":"outlawed",
		"author":"anna north",
		"tags":"A book about friendship"
	}
}

2.GET : http://localhost:8282/api/v1/library/load/19000
3.POST : http://localhost:8282/api/v1/library/upload
you need to select csv file which is available in src/main/resources
From POSTMAN : body ->form-data-> select KEY as file VALUE as select file like browse

4.PUT: http://localhost:8282/api/v1/library/update
{
	"bookDetails":{
		"id":1,
		"isbn":"1900001",			
		"title":"outlawed",
		"author":"anna north",
		"tags":"A book about friendship"
	}
}

5.DELETE : http://localhost:8282/api/v1/library/delete
{
	"bookDetails":{
		"id":1,
		"isbn":"1900001",			
		"title":"outlawed",
		"author":"anna north",
		"tags":"A book about friendship"
	}
}

