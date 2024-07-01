# curl (client URL)
this is my curl commands cheat sheet

# check http header info
curl -I http://127.0.0.1

![image](https://github.com/ehsanDadashi/curl/assets/29996315/9798147e-aeb5-4276-bb51-c8f05e07a771)

# check header and content
curl -i http://127.0.0.1

![image](https://github.com/ehsanDadashi/curl/assets/29996315/e7b5642e-0bce-4984-9a8d-5d4ade050b1e)

# check all details 
curl -v http://127.0.0.1

![image](https://github.com/ehsanDadashi/curl/assets/29996315/751ea0c5-f533-4b74-93b1-318b47f31a0d)

# tell curl to don't check if certificate is valid or not
curl -k https://127.0.0.1
![image](https://github.com/ehsanDadashi/curl/assets/29996315/310d1e11-d6f6-4f8c-ba52-4af95ecea870)

# work with api 
# get without input
 curl https://dummy.restapiexample.com/api/v1/employee/1
 ![image](https://github.com/ehsanDadashi/curl/assets/29996315/d4f3e0a2-767b-4f9e-b41a-56f9e44c9683)

 # post some data in query sting format . this format is default in post method in curl 
 curl -d "name=ehsan&salary=2000&age=33" https://dummy.restapiexample.com/api/v1/create
![image](https://github.com/ehsanDadashi/curl/assets/29996315/1b5644d4-9a6e-4e6c-842c-ea9287dc68a2)

# post some data with json format
curl -d '{"name":"ehsan","salary":"4000","age":"34"}' -H "Content-Type: application/json"  https://dummy.restapiexample.com/api/v1/create
![image](https://github.com/ehsanDadashi/curl/assets/29996315/5f949a89-3932-4d9e-955a-475c77502272)

# you can tell curl name of http method
curl -X POST -d '{"name":"ehsan","salary":"4000","age":"34"}' -H "Content-Type: application/json"  https://dummy.restapiexample.com/api/v1/create;
![image](https://github.com/ehsanDadashi/curl/assets/29996315/82374965-8058-4045-abfe-01506f320ee9)
