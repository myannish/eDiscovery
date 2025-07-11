How ngrok Works (Simple Explanation)
When you run: 	ngrok http 8080
ngrok:
	1. Opens a secure tunnel from your local machine to the internet.
	2. Generates a public URL (e.g., https://abc123.ngrok-free.app)
	3. Forwards all incoming traffic from that URL to your local port (e.g., http://localhost:8080)

This means:
	1. Your machine stays the server
	2. ngrok is just a proxy relay
	3. Files like .docx never leave your machine unless someone accesses them via your ngrok URL
