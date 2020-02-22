# HttpPostMan V 1.0.0 :
This JAR is a http request sender support a token bearer and all type of request (GET-POST-DELETE-PUT) From any Servlet to PHP native
or Framwork (laminas znend symfony ...) . 

## Import this JAR : 
is simple just add jar in your Project
![alt text](https://github.com/aboujaafar1997/HttpPostMan/blob/master/AddJAR.png)
## How to use :

###

    HashMap<String, String> params = new HashMap<String, String>();
		params.put("user", "me@example.com");
		params.put("password", "12345");
		HttpPostMan.newRequest(null, null, "http://localhost:8081/zend/zend.php", HttpPostMan.METHOD_POST, params,new Callback() {
			
			@Override
			public void OnSuccess(String response) {
				System.out.println("Res secuses = "+response);
				
			}
			
			@Override
			public void OnError(int status_code, String message) {
				System.out.println("Res err code= "+status_code+" message ="+message);
				
			}
		});

	}
###
