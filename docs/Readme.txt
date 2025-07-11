1. System Requirements
A. Server Environment
	OS: Windows 10/11 or Ubuntu 20.04+
	Java 8+ (for running Tomcat)
	Apache Tomcat 9+
	Docker (for ONLYOFFICE Document Server)

B. Tools & Dependencies
	Apache Tomcat
	Docker & Docker Desktop
	ngrok CLI
	ONLYOFFICE Document Server (Docker)
	Browser (Chrome, Edge)

2. ONLYOFFICE Setup (Docker)
Pull Docker Image: 	docker pull onlyoffice/documentserver
Run Document Server: 	docker run -i -t -d -p 80:80 onlyoffice/documentserver
Verify: 		Open http://localhost:8000/ in browser — ONLYOFFICE UI should load.


3. Expose Localhost with ngrok 
Download and Install ngrok: 		https://ngrok.com/download
Authenticate (first-time only): 	ngrok config add-authtoken <YOUR_AUTH_TOKEN>

Expose Tomcat Port (usually 8080): 	ngrok http 8080
Note the HTTPS URL: 			Forwarding https://abc123.ngrok-free.app -> http://localhost:8080

4. OnlyOffice Viewer integration ( in viewer.html)




