## API QUERY FOR THOR: RAGNAROK MOVIE USING GENERATED API KEY AND I PARAMETER

#how key was generated
#tool used for the purpose of this task
#brief description of tool
#attach postman script

API Query for Thor: Ragnarok:

GET http://www.omdbapi.com/?apikey=7805815b&i=tt3501632

//test for success

tests["Status code is 200"] = responseCode.code === 200;

//interogate response body

var jsonData = JSON.parse(responseBody);

//test expected 

tests["Title Matches"] =  responseBody.has("Thor: Ragnarok");

tests["Year Matches"] = responseBody.has ("2017");

tests["ID Matches"] = responseBody.has ("tt3501632");

## Tesct case

