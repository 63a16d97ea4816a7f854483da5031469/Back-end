## jersey warning when using @FormParam

##Warning:
<font color="red">Jan 14, 2016 4:03:52 PM com.sun.jersey.spi.container.servlet.WebComponent filterFormParameters
WARNING: A servlet POST request, to the URI http://localhost:8080/Que/appAPI/registerUser, contains form parameters in the request body but the request body has been consumed by the servlet or a servlet filter accessing the request parameters. Only resource methods using @FormParam will work as expected. Resource methods consuming the request body by other means will not work as expected.</font>

##Solved:
http://stackoverflow.com/questions/16848180/wrapping-request-parameters-using-httpservletrequestwrapper

Right. So I've been suffering this issue, and I've been trying to solve it on different ways, but I did't want to change my web.xml settings, just because if I was testing my application with Postman it worked perfect, but when it was being integrated with the webapp it fails with the mentioned issue (A servlet request to the URI {MY_URI} contains form parameters in the request body but the request body has been consumed by the servlet or a servlet filter accessing the request parameters. Only resource methods using @FormParam will work as expected. Resource methods consuming the request body by other means will not work as expected.)

So as @clijk mentioned, you only have to set your headers as:

"Content-Type": "application/json" 
"charset": "UTF-8" 
then, The warning it's gone.

Thanks
